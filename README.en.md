# Assessment Item Writer

**A Claude skill that writes test and exam questions that measure what they claim to measure.**

🇧🇪 [Nederlandstalige versie](README.md) · 📄 [Examples](examples/)

Give the topic or learning outcomes (ideally with the course material), the learners' level and the purpose of the test, and get questions an experienced test developer would sign off on: with answer key, feedback per option, and tags for outcome and cognitive level.

It works in English, Dutch and French: it replies in the language you write in.

## What the skill does

- **Avoids typical AI-question flaws:** trivia recall, the longest option being correct, obviously wrong distractors, "all of the above".
- **Builds a test blueprint** (outcomes × cognitive levels) for larger sets.
- **Plausible distractors** based on real misconceptions, so wrong answers are diagnostic.
- **Open questions** with a model answer and a scoring guide with partial credit.
- **Reviews existing questions** item by item, with improved versions.

## What you get

1. **Blueprint** (for larger sets)
2. **Questions** tagged [outcome · level · difficulty]
3. **Answer key and feedback** per option
4. **Quality notes**

See [examples/](examples/) for a full input and output.

## Who it's for

Teachers, lecturers, e-learning developers and trainers who write tests, exams, practice questions or knowledge checks.

This skill is part of **[Claude Skills for Education](https://github.com/ThomasAiluminated/claude-skills-for-education)**, an open collection for education and L&D:
- [Edu Prompt Coach](https://github.com/ThomasAiluminated/edu-prompt-coach): ready-to-paste prompts for teachers, with the pedagogy behind them
- [Lesson Designer](https://github.com/ThomasAiluminated/lesson-designer): lessons designed from objective to exit check
- [Rubric Builder](https://github.com/ThomasAiluminated/rubric-builder): assessment rubrics with observable levels
- [Feedback Writer](https://github.com/ThomasAiluminated/feedback-writer): specific, actionable feedback on student work
- [Inclusive Lesson Adapter](https://github.com/ThomasAiluminated/inclusive-lesson-adapter): accessible lesson materials using UDL
- [Learning Program Designer](https://github.com/ThomasAiluminated/learning-program-designer): training programs and learning journeys
- [Prompt Architect](https://github.com/ThomasAiluminated/prompt-architect): rough requests turned into strong prompts for Claude

## Install

**In Claude (web, desktop or mobile):**
1. Download [`assessment-item-writer.skill`](assessment-item-writer.skill)
2. Upload it under Skills in your Claude settings
   (or open the file in a Claude conversation and click *Save skill*)

**In Claude Code:** copy the `assessment-item-writer/` folder to `~/.claude/skills/`.

Then just ask, for example *"10 multiple-choice questions on photosynthesis for 14-year-olds"*. The skill starts automatically.

## Contributing

Ideas and improvements are welcome via an issue or pull request.

## License

[CC BY 4.0](LICENSE): free to use, adapt and share, with attribution.

---

Made by **Thomas Donvil**, [Ailuminated](https://ailuminated.org), AI literacy for education.
