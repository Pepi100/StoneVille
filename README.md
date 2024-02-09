<h1 align = "center">
StoneVille
</h1>

<h4 align = "center" >
  StoneVille este in joc interactiv care te plasează în rolul principal al arhitectului unui oraș medieval în plină creștere. În acest joc de strategie, vei construi orașe într-o lume medievală, pline de străzi înguste și piețe aglomerate, având grijă să satisfaci nevoile cetățenilor și să gestionezi resursele și infrastructură. Alegând între materiale tradiționale, vei evolua de la căsuțe simple la piețe impresionante și castele care să protejeze orașul. Misiunea ta este să creezi un oraș prosper și bine structurat, gestionând resursele pe care le ai la dispoziție.
</h4>



# Tasks

### Etapa 0

- (0.02) Alegerea temei (găsirea unui titlu pentru joc)

- Descrierea succintă a temei (google docs, 1/2-1 pagina). Va contine următoarele informații:

  - (0.13) o descriere generală a jocului (0.13 impartit in) :
    - (0.05) Contextul ( cadrul, povestea jocului; despre ce este vorba)
    - (0.03) În ce categorie se încadrează (strategie, shooter, adventure, fighting etc.). Pot fi categorii combinate.
    - (0.05) Regulile de joc: care sunt acțiunile posibile ale jucătorului. În ce situații se termină jocul. Cum se decide dacă a câștigat sau pierdut, cum se calculează eventualul scor.
 - (0.1) Stabilirea interacțiunii cu utilizatorul. Poate fi dată ca descriere în cuvinte sau diagramă UML (doar pentru acțiunile principale, nu tot jocul). Aceasta trebuie să cuprindă scenarii de utilizare. Care e prima interfață pe care o vede utilizatorul. Ce acțiuni disponibile are când intră în aplicație etc.
  - (0.02) Identificarea categoriei de utilizatori (vârstă, personalitate, interese, cadru social). Exemplu: jocul este dedicat vegetarienilor de toate vârstele, cu nivel mediu spre ridicat de cultură generală, pasionați de gătit, strategie și ecologie 😀
  - (0.03) Stabilirea cuvintelor/sintagmelor cheie (o lista cu minim 5-6 cuvinte cheie care descriu jocul). Motiv: unele platforme pentru publicarea jocurilor cer astfel de sintagme cheie (keywords, tags etc.)
  - (0.2) Căutarea unor jocuri similare (4-5 jocuri) ca temă pentru a observa lucrurile pro și contra (minim 2 aspecte pozitive și minim 2 aspecte negative pentru fiecare joc. Jocurile pot fi evaluate fi pe baza unui demo, a vizionării unor streaming-uri sau videoclipuri gratuite care arată desfășurarea jocului, și chiar cu ajutorul review-urilor.


  ### Etapa 1 - scenă simplă -  plasarea terenului, skyboxului și a altor elemente statice simple


  - [ ] (0.05) În scenă trebuie să existe un teren. Nu este obligatorie deplasarea pe teren, poate servi drept peisaj în jurul platformei de joc.

  - [ ] (0.15) Terenul trebuie să aibă un relief variat(să existe multiple zone joase și înalte). Terenul va avea alocat un material ce cuprinde multiple (minim 3) texturi (de exemplu, textură de iarbă, de nisip, de rocă etc). Texturile asociate trebuie pictate pe teren astfel încât să fie în concordanță cu forma terenului (de exemplu o groapă adâncă va avea textură de rocă și nu cu iarbă/floricele)

  - [ ] (0.05) Pe teren trebuie să existe minim o rampă (meniul Sculpt-> ramp)
- [ ] (0.05) Pe teren trebuie să existe două zone simetrice (de exemplu doi munți). (vezi meniul Sculpt-> mirror)

Cerințe materiale

- [ ] (0.05) Obiect cu material transparent
- [ ] (0.05) Obiect cu luciu metalic care reflectă mediul înconjurător
- [ ] (0.1) Obiect cu material lucios(care reflectă mediul) pe anumite zone și nelucios pe altele în funcție de un anumit pattern (rezolvarea se va face prin blueprints)
- [ ] (0.05) Existența unui obiect cu culoare emisivă.
- [ ] (0.05) Obiect care are un material cu gradient în 2 culori (gradientul se va realiza prin blueprints fără a folosi o textură externă)
- [ ] (0.05) Obiect care are transparență în gradient
- [ ] (0.15) Obiect care are un material cu gradient în 3 culori (gradientul se va realiza prin blueprints fără a folosi o textură externă)
- [ ] (0.1) Obiect care are un material transparent pe porțiuni și opac pe altele. Porțiunile de transparență sunt decise printr-un pattern (de exemplu altă textură)
- [ ] (0.1) combinarea culorilor a două texturi în funcție de un pattern dat de o a treia textură
- [ ] (0.2) simularea unei culori cu sclipici (puncte sclipitoare dispuse în mod aleator) folosind un nod de zgomot și fără folosirea unei texturi externe (adică a unei imagini)
- [ ] (0.15) Un material complex cu un pattern creat folosind minim 5 funcții matematice.
- [ ] (0.05) Folosirea unui normal map pentru a crea un obiect care dă senzația că are asperități chiar dacă nu și-a modificat vertecșii


### Meniu

- [x] (0.2p) La intrarea în joc se va afișa meniul principal al jocului. Jocul nu este pornit (de exemplu, este în pauză) până nu se iese din meniu.
- [ ] (0.05) Folosirea unei imagini într-un panou
- [x] (0.05) Folosirea panourilor de tip HorizontalBox și/sau VerticalBox
- [ ] (0.2p) Trecerea printre ecranele meniului folosind WidgetSwitcher
- [ ] (0.2-0.4p) Crearea unei clase custom pentru butoane. (se punctează în funcție de căt de complexă este.

Meniul principal poate conține următoarele butoane:
- [x] (0.2p)Butonul de pornire a unui joc nou. Butonul va avea un text sugestiv, de exemplu "Start". La intrarea în aplicație, jocul este în pauză, și rămâne așa până îl activează utilizatorul
- [ ] (0.3p)Butonul de continuare a ultimului joc început. La click pe acest buton, pornește jocul afișând exact starea în care a fost lăsat de utilizator înainte de ultima închidere (sau ultima salvare)
- [ ] (0.2p) Ecranul de setări generale (pentru profilul jucătorului sau caracteristicile unui joc nou. Ecranul de setări va fi accesat printr-un buton din meniul principal. Ecranul de setări va conține diverse inputuri și un buton de trimitere a datelor. La click pe buton setările se vor salva în proprietățile pionului/caracterului.

Inputurile folosite în ecranul de setări (sau alte ecrane care cer informații de la utilizator pot fi de următoarele tipuri (atenție, se punctează pentru fiecare tip distinct, nu input în sine):

- [ ] (0.05) EditableText
- [ ] (0.05) TextBox
- [ ] (0.1) Slider. Se vor seta parametri precum: valorile minime și maxime și pasul.
- [ ] (0.1) SpinBox. Se vor seta parametri precum: valorile minime și maxime, numrul de cifre zecimale, pasul (delta), exponentul de creștere (creșterea pasului pentru valori mai mari)

- [ ] (0.05) Checkbox
- [ ] (0.1) ComboBox cu minim 2 opțiuni
- [ ] (0.1) RadialSlider Se vor seta parametri precum: pasul, valoarea implicită etc.
- [ ] (0.1) Se dă suplimentar 0.1 pentru ComboBox dacă opțiunile sunt adăugate dinamic.
Se adună separat 0.1 pentru fiecare tip de input care e inclus într-un widget custom în scopul adăugării unor funcționalități noi la completare (Exemplu: un borderbox care își schimbă culoarea de background la fiecare apăsare de tastă

- [ ] (0 - 0.3)Aspectul ecranului de setări. Se acordă puncte în funcție de:
Cel mai important: Alinierea elementelor (de exemplu cu un grid)

Faptul că fiecare input are etichetă asociată (text în dreptul lui care să spună rolul) și/sau tool/tip,

Schimbarea culorilor implicite

Text lizibil (culori alese cu contrast bun; textul nu e prea transparent sau suprapus cu o imagine)

Folosirea unui background plăcut.

- [ ] (0.1) Adăugarea dinamică (prin program) a unor elemente în widget, folosind metode de tipul "Add Child to [container]"
- [ ] (0.1) Ștergerea dinamică (prin program) a unor elemente în widget, folosind metode de tipul "Remove Child"- [ ]
- [ ] (0.4p) Butonul de încărcare a unui joc vechi. La click pe acest buton se va deschide un ecran cu salvările anterioare ale utilizatorului din care acesta poate să aleagă ce joc dorește. Salvările pot fi listate prin butoane sau printr-un combobox. Ecranul va fi generat dinamic în funcție de fișierele din folderul de jocuri salvate. Identificarea jocurilor care corespund jucătorului curent se va face prin username.

Butonul de afișare a informațiilor despre joc:

- [ ] (0.1) va duce spre un ecran cu un text despre joc care explică povestea/contextul. Ecranul are un buton de revenire la meniul principal.

- [ ] (0-0.4) Stilizare specială a ecranului cu textul despre joc. Punctajul se dă în funcție de cât de complexă și frumoasă e stilizarea: 

folosirea unui scrollPane

folosirea culorilor diferite în cadrul textului

folosirea stilurilor diferite: bold/italic

stilizarea textului sub formă de secțiuni cu titluri

folosirea listelor

folosirea imaginilor în cadrul textului

- [x] (0.1p) Butonul de ieșire din aplicație (la click pe el se închide jocul)

- [ ](0.1) Cu ajutorul unui widget se va crea un meniu afișat pe parcursul jocului care va avea butoanele (punctate suplimentar după cum urmează):

- [ ] (0.1) Pauza - la Click pe el, jocul intră în pauză, iar când dăm iar click pe el reîncepe. Textul butonului ar trebui să difere în tipul pauzei, de exemplu să scrie "Reîncepe"

- [ ] (0.1) Un buton de ieșire din joc.
- [ ] (0.2) Un buton/shortcut cu tastă care pune în pauză jocul și afișează meniul principal. în această situătie meniul trebuie să aibă un buton suplimentar cu textul "Continua".

- [ ] (0.1-0.3) Afișarea informațiilor legate de starea jucătorului (sau a altor actori) în timpul jocului. Se punctează în funcție de cât de complexă e afișarea.

- [ ] (0.1) Folosirea unei bare de progres în afișarea informațiilor pentru jucător

- [ ] (0.2) Opțiunea de a ascunde și reafișa afișajul din timpul jocului, de exemplu, la apăsarea unei taste.

- [ ] (0.2) Simularea unor radio buttons folosind butoane custom

- [ ] (0.3) Simularea unor radio buttons folosind checkbox-uri custom

- [ ] (0.2-0.5) Unul sau mai multe ecrane informative care apar în urma unui eveniment sau a unei stări în care ajunge jocul. De exemplu, un ecran în care jucătorul e informat că a intrat într-un nivel nou sau că a "murit". Se punctează în funcție de numarul lor si de complexitatea afișării.

- [ ] (0.1) Buton de restart într-un ecran informativ, pentru cazul în care jucătorul a murit sau s-a terminat nivelul

- [ ] (0.2-0.4) Loading screen - se punctează în funcție de complexitate


Sunete (recomandat: 0.2 maxim:0.5)

- [ ] (0.1) Adăugarea unui sunet în cadrul jocului

Se punctează suplimentar:

- [ ] (0.1) Sunetul a apărut în cadrul unui widget în urma unui eveniment (de exemplu, click pe buton)

- [ ] (0.1) Sunetul a apărut în urma unei coliziuni

- [ ] (0.1-0.2) Sunetul depinde de acțiunile jucătorului și de mediu: deplasarea prin nisip generează alt sunet decât cea prin băltoace)
