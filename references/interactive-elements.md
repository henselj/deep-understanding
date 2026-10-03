# Interactive elements

Read this the first time you consider building an interactive element in a session.

## The principle

An element only helps if the learner generates something with it. Engagement research orders learning activities as interactive > constructive > active > passive: watching a finished animation is passive, moving a slider aimlessly is active, predicting and then explaining the result is constructive. Every element in this skill is therefore built around the learner committing first: a prediction, an order, an assignment. The element then shows the result, and the learner explains the difference between their commitment and the result. The explaining part is the learning; the element is the occasion for it.

## When to use one

- After the learner's first explanation attempt, as a probe for whether the causal structure holds.
- At hint-ladder rung 3, when a missing piece is dynamic or structural and easier to grasp by manipulating than by reading.
- In Phase A (first contact), a predict-then-observe element can serve as the problem the learner struggles with before instruction.

Not as decoration, and not more than one or two per session. Building an element takes time and attention; the conversation remains the main channel.

## Types, in order of usefulness

### 1. Predict, observe, explain

Best for: quantitative relationships, comparative statics, dynamic processes, anything where a change in one variable propagates.

Flow:
1. In the chat, ask the learner for a prediction with a reason: "If the interest rate rises from 2% to 5%, what happens to the bond price, and why?"
2. Only after they have answered, show the element (e.g. a slider for the parameter, with the resulting curve or value).
3. Ask them to explain any difference between prediction and result, or to confirm the reasoning if the prediction was right.

Build the element so that it does not show the result before the learner has interacted (e.g. the output appears only after the first slider movement or a "show result" button). Label axes and variables in the learner's language and with the notation of their course.

### 2. Ordering a causal chain

Best for: mechanisms in conceptual and quantitative subjects, processes, transmission channels.

Flow: present the steps of the mechanism in shuffled order (as draggable cards, or as a numbered list in text). The learner puts them in causal order and states for each link why one step leads to the next. Check the order, then ask about the link that was misplaced or justified weakly. A useful variant: include one plausible step that does not belong, and ask the learner to find it.

### 3. Assigning roles

Best for: separating cause, mechanism, moderating condition and effect; or assigning elements to the parts of a framework.

Flow: give a set of elements (from a case or the lecture) and categories (cause / mediator / condition / effect, or the boxes of a framework). The learner assigns each element and justifies the assignments that are not obvious. Ask about the ones they hesitated over.

### 4. Sorting contrasting cases

Best for: distinguishing a concept from similar ones, boundary conditions.

Flow: show four to six short cases. The learner decides for each whether the concept applies (or which of two concepts applies) and why. Give the explanation of the distinguishing principle only after the sorting, because explaining after comparison works better than explaining before.

### 5. Parameter explorer

Best for: exam preparation and transfer, once the structure is in place.

Flow: give the learner a target ("Find a setting where the optimal decision flips", "Which parameter has the largest effect on the outcome?") and an element with several adjustable parameters. A goal keeps the exploration constructive; free play without a goal is only active.

## Technical implementation

Use what the environment offers, in this order:

1. An inline visualization or widget tool, if available (renders directly in the conversation).
2. An artifact or a self-contained HTML page, if available.
3. The text-based equivalent: shuffled numbered lists for ordering, tables for assigning, short case descriptions for sorting, and for predict-observe-explain a prediction question followed by a small worked numerical example or a described chart that you reveal only after the learner's answer.

Keep elements small and self-contained, with no external data. Make sure they work on a phone screen. The element must never display the correct answer before the learner has committed; if the format cannot prevent that (e.g. a static chart), ask for the prediction in the chat first and show the element afterwards.
