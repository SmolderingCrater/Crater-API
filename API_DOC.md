`function speak(e, t) {
    var a = new SpeechSynthesisUtterance;
    a.text = e, a.onend = function() {
        t && t()
    }, a.onerror = function(e) {
        t && t(e)
    }, speechSynthesis.speak(a)
}'
