# Assessment Item Writer

**Een Claude-skill die toets- en examenvragen schrijft die meten wat ze beweren te meten.**

🇬🇧 [English version](README.en.md) · 📄 [Voorbeelden](examples/)

Je geeft het onderwerp of de leerdoelen (liefst met het lesmateriaal erbij), het niveau van je leerlingen en het doel van de toets, en je krijgt vragen terug die een ervaren toetsontwikkelaar zou goedkeuren: met sleutel, feedback per antwoordoptie en een koppeling aan leerdoel en cognitief niveau.

*English summary: a Claude skill that writes high-quality test and quiz questions (multiple choice with plausible distractors, open questions with model answers and scoring guidance), mapped to learning outcomes and cognitive levels, with an answer key and feedback per option. It works in Dutch, French and English.*

## Wat de skill doet

- **Vermijdt de typische zwaktes van AI-vragen:** feitjes in plaats van begrip, het juiste antwoord dat altijd het langste of meest precieze is, afleiders die duidelijk fout zijn, en "alle bovenstaande".
- **Maakt eerst een toetsmatrijs** bij meer dan een vijftal vragen: leerdoelen × cognitieve niveaus (onthouden, begrijpen, toepassen, analyseren, evalueren), met het zwaartepunt op begrijpen en toepassen.
- **Schrijft sterke meerkeuzevragen:**
  - een stam die zonder de opties te begrijpen is
  - afleiders gebaseerd op echte misconcepties, zodat foute antwoorden iets vertellen
  - geen weggevers: geen lengteverschil, geen grammaticale hints, geen "nooit/altijd" alleen in afleiders
  - korte casussen voor hogere denkniveaus
- **Schrijft open vragen** met een expliciete opdracht, een modelantwoord en een scoringswijzer met deelpunten.
- **Baseert de inhoud op jouw materiaal**, en markeert wat je best nog nakijkt tegenover je eigen cursus.
- **Reviewt ook bestaande vragen**, concreet en per vraag, met verbeterde versies.

## Wat je terugkrijgt

1. **Toetsmatrijs** (bij grotere sets)
2. **De vragen**, genummerd en getagd met [leerdoel · niveau · moeilijkheid]
3. **Sleutel en feedback** per antwoordoptie, voor formatief gebruik gericht aan de leerling
4. **Kwaliteitsnotities**: wat je zelf nog best controleert

Op vraag kan de skill de vragen ook exporteren naar een document, spreadsheet of een formaat voor je LMS of quiztool.

## Voor wie

Voor leerkrachten, docenten in het hoger onderwijs, e-learningontwikkelaars en trainers die toetsen, examens, oefenvragen of kennischecks maken, van basisonderwijs tot bedrijfsopleiding.

Deze skill hoort bij **[Claude Skills for Education](https://github.com/ThomasAiluminated/claude-skills-for-education)**, een open reeks voor onderwijs en L&D:
- [Edu Prompt Coach](https://github.com/ThomasAiluminated/edu-prompt-coach): prompts voor leerkrachten, met uitleg waarom ze werken
- [Lesson Designer](https://github.com/ThomasAiluminated/lesson-designer): lessen ontwerpen van leerdoel tot exit-check
- [Rubric Builder](https://github.com/ThomasAiluminated/rubric-builder): beoordelingsrubrics met observeerbare niveaus
- [Feedback Writer](https://github.com/ThomasAiluminated/feedback-writer): specifieke, haalbare feedback op leerlingenwerk
- [Inclusive Lesson Adapter](https://github.com/ThomasAiluminated/inclusive-lesson-adapter): lesmateriaal toegankelijk maken met UDL
- [Learning Program Designer](https://github.com/ThomasAiluminated/learning-program-designer): opleidingen en leertrajecten ontwerpen
- [Prompt Architect](https://github.com/ThomasAiluminated/prompt-architect): een ruwe vraag omzetten in een sterke prompt voor Claude

## Installeren

**In Claude (web, desktop of mobiel):**
1. Download [`assessment-item-writer.skill`](assessment-item-writer.skill)
2. Upload het bij de Skills in je Claude-instellingen
   (of open het bestand in een gesprek met Claude en klik op *Save skill*)

**In Claude Code:** kopieer de map `assessment-item-writer/` naar `~/.claude/skills/`.

Daarna volstaat een gewone vraag, zoals *"schrijf 10 meerkeuzevragen over fotosynthese voor het tweede middelbaar"*. De skill start vanzelf.

## Structuur

```
assessment-item-writer/
└── SKILL.md                    # de volledige instructies van de skill
examples/                 # voorbeelden van input en output
assessment-item-writer.skill    # installeerbaar pakket
```

## Bijdragen

Ideeën en verbeteringen zijn welkom via een issue of pull request.

## Licentie

[CC BY 4.0](LICENSE): vrij te gebruiken, aan te passen en te delen, met naamsvermelding.

---

Gemaakt door **Thomas Donvil**, [Ailuminated](https://ailuminated.org), AI-geletterdheid voor het onderwijs.
