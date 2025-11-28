# Iron Protocol Kettlebell

Questo repository contiene una singola pagina `index.html` con il generatore di programmi per kettlebell. Usa HTML, CSS e JavaScript nativi: non servono build tool o dipendenze.

## Come applicare gli aggiornamenti
1. **Recupera l'ultima versione**
   ```bash
   git checkout work
   git pull
   ```
2. **Sostituisci la pagina online**
   - Se usi GitHub Pages con una repository dedicata, copia l'attuale `index.html` in quella repo (sovrascrivendo la versione pubblicata).
   - In alternativa, pubblica direttamente questa repo su GitHub Pages (branch `main`/`master` o cartella `/docs`, in base alla tua configurazione).
3. **Verifica in locale** (opzionale ma consigliato)
   - Avvia un server statico dalla radice del progetto:
     ```bash
     python -m http.server 8000
     ```
   - Apri <http://localhost:8000> e testa il bottone **GENERA PROTOCOLLO** e il layout mobile ridimensionando la finestra o usando gli strumenti DevTools.
4. **Esegui il deploy**
   - `git add index.html` (o l'intera cartella, se hai spostato altri asset).
   - `git commit -m "Aggiorna pagina kettlebell"`.
   - `git push` verso il branch servito da GitHub Pages.
5. **Svuota la cache del browser**
   - Dopo il deploy, forza un hard refresh (Ctrl+F5 / Cmd+Shift+R) o apri la pagina in una finestra anonima per assicurarti di vedere gli ultimi stili.

## Note utili
- Il file `index.html` include già gli stili responsivi per ridurre lo scrolling orizzontale su mobile.
- Non sono necessari asset esterni oltre ai font Google inclusi via CDN.
