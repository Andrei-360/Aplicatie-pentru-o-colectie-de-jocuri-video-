# GameVault
Aplicație pentru gestionarea și evidența colecției personale de jocuri video.
Permite urmărirea jocurilor în desfășurare, a titlurilor finalizate, precum și a platformelor, genurilor și expansiunilor deținute.

## Model de date

| Câmp | Tip | Note |
| :--- | :--- | :--- |
| titlu | text | obligatoriu, max 100 caractere |
| finalizat | boolean | comutat din listă, implicit fals |
| platforma | valori fixe | PC, PlayStation, Xbox |
| gen | relație | RPG, Action, Shooter (categorie, din etapa 10) |
| expansiuni | text | opțional, expansiuni/DLC-uri deținute |
| utilizator | relație | proprietarul elementului (din etapa 11) |

Date de test utilizate în toate etapele:
1. The Witcher 3, activ, PC
2. Elden Ring, finalizat, PlayStation
3. Cyberpunk 2077, activ, Xbox

## Mod de rulare
Se deschide fișierul index.html într-un browser web. Nu necesită etapă de build sau server.

## Utilizare AI

| Instrument | Scopul utilizării |
| :--- | :--- |
| Gemini | Structurarea HTML semantic, layout CSS cu Grid/Flexbox, media queries și variabile pentru tema întunecată |

Detalii pentru fiecare etapă: consultați folderul ai-log/.

## Stadiu
- [x] Etapa 1: mockup static
- [ ] Etapa 2: logica pe date în JavaScript
