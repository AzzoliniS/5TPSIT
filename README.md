# Esempio di webservice CRUD RESTFUL

## Tecnologie utilizzate
Il webservice è realizzato in **Nodejs**, mentre il database utilizzato è **Mysql**.  
Il server mysql è in esecuzione in un container **Docker**.  
I parametri di configurazione del server sono definiti nel file <u>docker-compose.yml</u>.  

Per creare il container e mandarlo in esecuzione eseguire il comando:

>`docker-compose up -d`. 

> [!IMPORTANT]
>Durante la creazione del container (ovvero l'installazione di mysql), verrà anche creato il database definiti attraverso gli script presenti nella directory mysql

Se il container è già stato creato ed è fermo, lo si può avviare con il comando:

> `docker-compose start`

> [!NOTE]
>Per una comoda gestione dei container docker è consigliabile installare l'estensione **Docker** in Visual Studio Code.

## Procedura di installazione
1. Clonare il progetto nel proprio codespace o in una cartella del proprio PC: se si decide di sviluppare il progetto in locale, assicurarsi di aver installato **Nodejs** e **Docker desktop**:  
`git clone https://github.com/andreatrentini/esempio-restfull-node-mysql.git`
2. dopo aver clonato il progetto, mandare in esecuzione il server mysql con l'istruzione riportata sopra: `docker-compose up -d`
3. entrare nella cartella wsserver da terminale: `cd wsserver`
4. installare le librerie utilizzate dal progetto node: `npm install`
5. installare in modo globale **nodemon** (applicativo da utilizzare per mandare in esecuzione il server node in fase di svilippo: ad ogni cambiamento dei file presenti nella cartella il server viene riavviato): `npm install -g nodemon`
6. avviare il server: `nodemon app.js`

## Test del webservice
Per testare il server, è possibile installare in **Visual Studio Code** l'estensione chiamata **REST Client**, e inviare le richieste http presenti nel file **http-request.http**.
Al file è possibile aggiungere altre richieste.  
>NB: Fra una richiesta e l'altra deve essere presente il separatore ###

## Documentazione
Il codice presente nel file **app.js** è interamente commentato e riporta il significato delle istruzioni presenti.

## Link interessanti
### Docker
- [Docker](https://www.docker.com/)
- [Docker desktop](https://www.docker.com/products/docker-desktop/)
- [Docker compose](https://docs.docker.com/compose/)
- [Immagine ufficiale di MYSQL](https://hub.docker.com/_/mysql)
### Node
- [Nodejs](https://nodejs.org/en)
- [Express](https://expressjs.com/it/)
- [Nodemon](https://www.npmjs.com/package/nodemon)
### Riferimenti teorici web
- [RESTFul WEB Services](https://www.html.it/guide/restful-web-services-la-guida/)
- [Una guida per principianti all'HTTP e REST](https://code.tutsplus.com/it/a-beginners-guide-to-http-and-rest--net-16340t)
- [Wikipedia: HTTP](https://it.wikipedia.org/wiki/Hypertext_Transfer_Protocol)

  
    
  
**Buon divertimento!!!**