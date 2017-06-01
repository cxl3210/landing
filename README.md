# landing
# landing

playPrevious:function(){
  var index=this.attributes['index'];
  index=index-1;
  if(index===-1){
    if(this.attributes['loop']){
      index=audioData.length-1;
    }else{
       this.handler.state = constants.states.START_MODE;
       var message = 'You have reached at the start of the playlist.';
       this.response.speak(message).audioPlayerStop();
       return this.emit(':responseReady');
    }
  }
    this.attributes['index'] = index;
    this.attributes['offsetInMilliseconds'] = 0;
    this.attributes['playbackIndexChanged'] = true;
    controller.plays.call(this);
}


play:function(){
  this.attributes['state']='PLAYMODE';
  if (this.attributes['playbackFinished']) {
      this.attributes['index'] = 0;
      this.attributes['offsetInMilliseconds'] = 0;
      this.attributes['playbackIndexChanged'] = true;
      this.attributes['playbackFinished'] = false;
  }
}

var audioEventHandlers=function(){
   'PlaybackFinished' : function () {
        this.attributes['playbackFinished'] = true;
        this.attributes['enqueuedToken'] = false;
        this.emit(':saveState', true);
}
