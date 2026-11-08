# Muffinbot

<p align="center">
  <img src="assets/muffinbot-icon.jpg" alt="Muffinbot's original chocolate-chunk muffin illustration" width="320">
</p>

> An experimental, local-first artificial intelligence exploring language, reasoning, memory, emotion-like state, and learning through experience.

Muffinbot is the name of the AI and the project. Its visual identity is the user's supplied illustrated chocolate-chunk muffin character, preserved as `assets/muffinbot-icon.jpg`.

## Project vision

Muffinbot is not intended to be only a question-answering chatbot. It is an experimental modular agent whose language and personality are connected to internal systems for:

- **Intelligence:** reasoning, planning, problem-solving, and evaluating options.
- **Personality:** a starting temperament that can gradually evolve through accumulated experience.
- **Emotion-like state:** contextual variables such as fear, happiness, sadness, curiosity, and trust that influence decisions and communication.
- **Memory:** short-term working context and persistent long-term episodic/semantic memories.
- **Learning:** updating associations, strategies, and behavioural tendencies based on outcomes.
- **Environment:** a safe sandbox where Muffinbot can explore, act, receive feedback, and learn from consequences.

These mechanisms model emotion and adaptive behaviour. They do not, by themselves, establish consciousness or subjective feelings.

## Design principles

1. **Local-first:** prioritize running on consumer hardware and Android; use cloud services only as optional extensions.
2. **Modular:** keep language, reasoning, emotion, memory, learning, and interface components independently testable.
3. **Inspectable:** make internal state changes, memories, and decisions observable during development.
4. **Adaptive, not blindly agreeable:** Muffinbot can question assumptions, explain disagreement, and revise beliefs when evidence changes.
5. **Permissive discussion with safeguards:** support mature topics, profanity, dark humor, and controversial discussion while refusing sexualization of minors, extreme graphic violence, and actionable assistance for real-world harm.
6. **No fake sentience claims:** describe implemented behaviour accurately and distinguish simulation from demonstrated subjective experience.

## Proposed architecture

```text
Muffinbot/
├── assets/
│   └── muffinbot-icon.jpg
├── brain/
│   ├── intelligence/    # reasoning and decision support
│   ├── personality/     # traits and long-term temperament
│   ├── emotions/        # contextual affective state
│   ├── memory/          # working, episodic, and semantic memory
│   └── learning/        # adaptation from feedback and outcomes
├── language/            # language model interface and dialogue
├── environment/         # sandbox, actions, observations, rewards
├── android/             # Android integration and on-device runtime
├── tests/
└── docs/
```

This is the planned structure, not a claim that these modules have already been implemented.

## Initial technology direction

- **Python:** prototype the brain, experiments, evaluation, and model integration.
- **Kotlin:** Android application and device integration.
- **C++ (optional):** performance-critical components if profiling shows a need.
- **Small / quantized language model:** provide language capability within mobile memory and compute limits.

The final model and runtime will be selected after benchmarking on the target device.

## Development roadmap

- [ ] Define core interfaces and a minimal runnable project.
- [ ] Build a dialogue loop with a replaceable language-model backend.
- [ ] Implement contextual emotion variables and state transitions.
- [ ] Add working and persistent memory.
- [ ] Add experience-based learning and evolving personality traits.
- [ ] Build a sandbox for actions, consequences, and evaluation.
- [ ] Benchmark and package an Android prototype.

## Status

**Stage:** project setup and architecture design.

The artwork is referenced above and is to be committed at `assets/muffinbot-icon.jpg`. No intelligence, emotion, or learning modules are claimed as implemented yet. Progress will be recorded as working code and tests are added.
