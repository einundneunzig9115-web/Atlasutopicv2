# Atles Utòpic de Poti · v0.26

Actualització centrada en la fiabilitat de les recomanacions individuals del test.

## Què canvia en aquesta versió

- **Menys pes per etiquetes genèriques.** La puntuació combina la freqüència d'una etiqueta entre els perfils del catàleg amb la freqüència amb què apareix en opcions de resposta del mòdul. Les idees que no es pregunten en un mòdul no poden aportar-hi puntuació.
- **Signatures doctrinals individuals.** Les 72 fitxes de referència individual amb què s'ha treballat (17 de política, 32 de consciència i 23 d'existència) disposen d'un conjunt de trets nucli. Per recomanar un nom, el test requereix coincidències en almenys tres preguntes, com a mínim dos trets mesurats i almenys un tret prou distintiu dins de les fitxes seleccionades.
- **Requisit específic per a Philip Pettit.** La recomanació requereix evidència repetida tant de no-dominació com de poder impugnable i revisable. «Ordre», «igualtat» o «Estat protector» ja no poden funcionar per si sols com a substituts de la seva tesi central.
- **Abstenció quan hi ha empat.** Si dos resultats individuals qualificats queden massa a prop, no es força un nom: es mostren les afinitats temàtiques i s'indica que la comparació individual no és concloent.
- **Correcció del resultat ambigu.** La vista de resultats ja no torna a validar accidentalment el primer element del rànquing brut quan el filtre d'evidència no ha acceptat cap candidat.
- **Concepte nou traduït** als tres idiomes de la web: català, castellà i anglès.

## Prova de diagnòstic reproduïble

S'han provat 300 patrons sintètics de respostes polítiques, amb la mateixa seqüència pseudoaleatòria per comparar la lògica anterior i la nova:

- Amb la lògica v0.25, Philip Pettit era el primer resultat individual qualificat en el **27,0 %** de les mostres.
- Amb la lògica v0.26, ho era en el **6,0 %**.
- La v0.26 no assignava un autor individual en el **39,7 %** de les mostres sintètiques, perquè les respostes no oferien prou evidència específica o diferenciada.

També s'han comprovat perfils de resposta construïts expressament: el perfil republicà de no-dominació apunta a Pettit, el minarquista a Robert Nozick, el policèntric a James C. Scott i l'anarquista a Piotr Kropotkin. Un patró autoritari ambigu no força un autor concret.

**Important:** aquests són tests sintètics de codi, no una mostra de persones reals ni una mesura de precisió psicològica. La millora redueix resultats massa segurs quan falten senyals diferenciadors; no demostra que un test de 33 preguntes pugui identificar definitivament una persona o totes les seves conviccions. Quan una tesi distintiva d'un pensador no es pregunta explícitament, és preferible no atribuir-li un resultat individual.

## Publicar a GitHub Pages

1. Descomprimeix el ZIP.
2. Substitueix l'`index.html` del directori arrel del repositori pel que hi ha al ZIP.
3. Fes *commit* i *push* dels canvis.
4. Espera que GitHub Pages acabi el desplegament i recarrega la web. Si el navegador manté la versió anterior, fes una recàrrega completa.

`README.md` és documentació opcional; la pàgina web funciona amb `index.html`.
