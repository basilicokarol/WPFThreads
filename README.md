# WPFThreads
Lambda Expression
 fornisce un elenco di parametri formali e un corpo che può essere un'espressione o un blocco di codice. Le espressioni lambda risolvono il problema della verbosità delle classi interne permettendo una riduzione delle linee di codice da scrivere.
 c# lock
 L'istruzione lock acquisisce il blocco a esclusione reciproca per un oggetto specificato, esegue un blocco di istruzioni e quindi rilascia il blocco. Mentre è attivo un blocco, il thread che contiene il blocco può ancora acquisire e rilasciare il blocco. Gli altri thread non possono acquisire il blocco e devono attendere finché il blocco non viene rilasciato. L'istruzione lock garantisce che un singolo thread abbia accesso esclusivo a tale oggetto.
 object __lockObj = x;
bool __lockWasTaken = false;
try
{
    System.Threading.Monitor.Enter(__lockObj, ref __lockWasTaken);
    // Your code...
}
finally
{
    if (__lockWasTaken) System.Threading.Monitor.Exit(__lockObj);
}


