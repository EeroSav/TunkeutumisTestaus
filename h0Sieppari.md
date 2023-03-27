# h0 Sieppari ruispellossa

Sieppaa ja analysoi verkkoliikennettä.

analysoin verkkoliikennettä firefoxin network työkalulla jonka sain auki f12 nappia painamalla.

![TTPictures/H0-1.png]()

Kaikki get pyyntöjä, 
304 client redirection message
200 OK 

avatussa get pyynnössä pyydetty tiedosto `/portal/wikipedia.org/assets/js/index-86c7e2579d.js`

![TTPictures/H0-2.png]()


age:2758

The Age header contains the time in seconds the object was in a proxy cache.

The Age header is usually close to zero. If it is Age: 0, it was probably fetched from the origin server; otherwise, it was usually calculated as a difference between the proxy's current date and the Date general header included in the HTTP response. 

Koska haettu etusivu, ei vastausta ole tarvittu päivittää serveriltä vaan se on ollut tallessa proxy palvelimella.

![TTPictures/H0-3.png]()

lisää tutkittuani oletin että ensimmäinen 304 redirect pyyntö oli oleellisempi analysoitava  

filename: oikea etusivu ja age 80106 vastaa muutamaa päivää  
Address: palvelimen osoite  
