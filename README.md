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


