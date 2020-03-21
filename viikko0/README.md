0.4: uusi muistiinpano

selain->palvelin:HTTP POST fullstack-exampleapp.herokuapp.com/new_note

note over palvelin:
uusi viesti lähetetään selaimelta palvelimelle
end note

palvelin-->selain: HTML

selain->palvelin:HTTP GET fullstack-exampleapp.herokuapp.com/notes
palvelin-->selain: HTML

selain->palvelin: HTTP GET fullstack-exampleapp.herokuapp.com/main.css
palvelin-->selain: main.css

selain->palvelin: HTTP GET fullstack-exampleapp.herokuapp.com/main.js
palvelin-->selain: main.js

selain->palvelin: HTTP GET fullstack-exampleapp.herokuapp.com/data.json
palvelin-->selain: json tiedosto

note over selain:
uusi viesti on nyt muiden
viestien joukossa ja selain näyttää viestit.
end note

-----------------------------------------------------------------------
0.5: Single Page App

selain->palvelin: HTTP GET fullstack-exampleapp.herokuapp.com/spa
palvelin-->selain: HTML
selain->palvelin: HTTP GET fullstack-exampleapp.herokuapp.com/main.css
palvelin-->selain: main.css
selain->palvelin: HTTP GET https://fullstack-exampleapp.herokuapp.com/spa.js
palvelin-->selain: spa.js
selain->palvelin: HTTP GET fullstack-exampleapp.herokuapp.com/data.json
palvelin -->selain: json tiedosto

-----------------------------------------------------------------------

0.6: Uusi muistiinpano

selain->palvelin: HTTP POST https://fullstack-exampleapp.herokuapp.com/new_note_spa
palvelin -->selain: json tiedosto