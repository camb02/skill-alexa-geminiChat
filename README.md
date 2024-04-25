#Alexa GeminiChat
### Alexa Skill Template per integrare Google Gemini sui dispositivi Alexa

**Visita il canale [Scintilla Hub](https://www.youtube.com/@scintillahub) su YouTube**

## Requisiti
* Con un account Google, genera una chiave di autenticazione API sul sito web di [Google AI Developer] (https://ai.google.dev/). Copia e salva la chiave, sarà visibile solo al momento della creazione.
* Crea un account su [Amazon](https://www.amazon.com/ap/signin?openid.pape.preferred_auth_policies=Singlefactor&clientContext=132-2293245-7926858&openid.pape.max_auth_age=7200000&openid.return_to=https%3A%2F %2Fdeveloper.amazon.com%2Falexa%2Fconsole%2Fask&openid.identity=http%3A%2F%2Fspecs.openid.net%2Fauth%2F2.0%2Fidentifier _select&openid.assoc_handle=amzn_dante_us&openid.mode=checkid_setup&marketPlaceId=ATVPDKIKX0DER&openid.claimed_id=http% 3A %2F%2Fspecs.openid.net%2Fauth%2F2.0%2Fidentifier_select&openid.ns=http%3A%2F%2Fspecs.openid.net%2Fauth%2F2.0&) e accedi alla _Console per sviluppatori Alexa_.
## Creazione dell'abilità Alexa
Creare una Skill ospitata da Alexa (Python) su Alexa: (_Create Skill_)

1. Dai un nome alla tua abilità: scegli un nome a tua scelta (Es: GeminiGPT)
2. Scegli una lingua principale: Italiano 
3. Fare clic su _Avanti_. Nel tipo di esperienza seleziona: Altro > Personalizzata > _Ospitato su Alexa (Python)_
4. _Regione di hosting_: puoi lasciare la regione predefinita _Stati Uniti orientali (Virginia settentrionale)_
5. In _Modelli_: fai clic su _Importa competenza_
6. Inserisci l'indirizzo del repository: https://github.com/camb02/skill-alexa-geminiChat.git e conferma.

## Configurazione dell'abilità
Al termine dell'importazione in _Invocazioni_ > _Nome chiamata abilità_:
1. Modifica _Nome chiamata abilità_. Questo sarà il comando di invocazione per la tua abilità. Soddisfa i requisiti e le restrizioni sulle parole
2. Fai clic su _Salva_
3. Sviluppa l'abilità facendo clic su _Crea abilità_. Al termine, vai alla scheda **Codice**
4. Crea un file all'interno della cartella Lambda chiamato _.env_ e aggiungi la riga, aggiungendo la chiave API generata:
    "conchiglia".
    GOOGLE_API_KEY=YourApiKeyGoogleAI
    ```
5. Fai clic su _Salva_ e poi su _Distribuisci_
   
## Prova di abilità
Al termine della _deploy_, vai alla scheda **Test**:
1. In _Il test delle competenze è abilitato nel_ passaggio da _Off_ a _Sviluppo_
2. Per utilizzare i comandi vocali, accetta la richiesta del sito Web di utilizzare il microfono e, per parlare, fai clic e tieni premuta l'icona del microfono e rilascia per inviare
3. Utilizza il comando di attivazione configurato per avviare la Skill e sei pronto per interagire con Gemini tramite Alexa!

La Skill sarà ora disponibile su tutti i dispositivi Alexa collegati al tuo account.
