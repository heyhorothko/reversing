
<body>
<div class="inner-content">
<script charset="utf-8" type="text/javascript" src="https://static.polldaddy.com/p/9794855.js"></script>
</div>
</body>

<script>
window.alert = function(msg) {
     console.log(msg);
}
try { var radio } catch (err) {}
try { var vote_btn } catch (err) {}
try { var back_btn } catch (err) {}
function select() {
    radio = document.getElementById('PDI_answer44811657')
    vote_btn = document.getElementById('pd-vote-button9794855')
    back_btn = document.querySelector('a.pds-return-poll')
}
function eventFire(el, etype){
  if (el.fireEvent) {
    el.fireEvent('on' + etype);
  } else {
    var evObj = document.createEvent('Events');
    evObj.initEvent(etype, true, false);
    evObj.which = el
    el.dispatchEvent(evObj);
  }
}
setInterval(function() { 
    select()
    try { 
        radio.click()
        eventFire(vote_btn, 'click')
    } catch (e) {  }
}, 3000)
setInterval(function() {
    select()
    try { back_btn.click() } catch (e) {  }
}, 10000, 500)
setInterval(function () {window.location.reload()}, 5*60000);
</script>
 Desktop version
