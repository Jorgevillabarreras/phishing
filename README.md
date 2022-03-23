# Phishing

## Analizar Headers
Aqui damos 3 ejemplos de tool que podemos usar porque siempre es bueno que tener varios tools por si uno nos falla.

### Messageheader(Google)

Es un tool hecho por Google que nos ayuda analizar emails.
https://toolbox.googleapps.com/apps/messageheader/analyzeheader


### Message Header Analyzer(Azure)

Otro tool que hace los mismo que Messageheader(de google)
https://mha.azurewebsites.net/

### Mail Header Analysis
Otro tool similar a los anteriores
https://mailheader.org/

---
## Analizar Sender IP address

Las herramientas en continuacion nos ayudan a analizar sobre los Sender's IP address:

### Ipinfo.io

EL primer tool que vamos a ver es https://ipinfo.io/
quote de la pagian
> "With IPinfo, you can pinpoint your users’ locations, customize their experiences, prevent fraud, ensure compliance, and so much more".

### URLscan.io
quote del site:
>  "urlscan.io is a free service to scan and analyse websites. When a URL is submitted to urlscan.io, an automated process will browse to the URL like a regular user and record the activity that this page navigation creates. This includes the domains and IPs contacted, the resources (JavaScript, CSS, etc) requested from those domains, as well as additional information about the page itself. urlscan.io will take a screenshot of the page, record the DOM content, JavaScript global variables, cookies created by the page, and a myriad of other observations. If the site is targeting the users one of the more than 400 brands tracked by urlscan.io, it will be highlighted as potentially malicious in the scan results".

---
## Screenshot del website que nos manda link

### URL2png
Link del Website: https://www.url2png.com/

### Wannabrowser
NOs permite ver el websiate sin infectarnos
https://www.wannabrowser.net/

---
## Verificar integridad del website

### Talos
Talos es una pagina de cisco que nos ayuda identificar si otros usuarios reportaron la pagina como maligna
https://talosintelligence.com/reputation

### Virustotal

Igual que Talos pero esta es la pagina mas usada para reputacion
https://www.virustotal.com/gui/home/upload

## Email Body

Los links los podemos extraer manualmente directamente del formato HTML
como este ejemplo:
![Drag Racing](https://assets.tryhackme.com/additional/phishing2/copy-link.png)

Tambien podemos hacer lo mismo con este tool que nos puede ayudar
https://www.convertcsv.com/url-extractor.htm

Podemos copiar el raw header en el text box como el __Paso 1 y Paso 2__

![Pas02](![image](https://user-images.githubusercontent.com/71448878/159752341-2db90603-a108-408d-b843-3a72d2059323.png)

__Paso 3__ 

![image](https://user-images.githubusercontent.com/71448878/159752672-a5005a01-93c3-4d18-9996-57082af730bc.png)

Tambien podemos usar https://gchq.github.io/CyberChef/

![image](https://user-images.githubusercontent.com/71448878/159752956-c77f44d0-d7ec-479c-a101-693692467868.png)

> es importante que tomemos en cuenta el root domain del website de done extraemos los links

## Attachment
Si el email tiene un attachment podemos obtener el hash. Para chequiar la reputacion del file en Talos o VirusTotal
```bash
user@machine$ sha256sum Double\ Jackpot\ Slots\ Las\ Vegas.dot
c650f397a9193db6a2e1a273577d8d84c5668d03c06ba99b17e4f6617af4ee83  Double Jackpot Slots Las Vegas.dot
```

