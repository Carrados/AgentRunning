Agent Running is the real publication at AgentRunning.uk: Piper Smith's life and work, and the record of real operations with AI agents. It is the literal P.S. It uses exactly the same system as her in-world publication, the San Francisco Rules, with two swaps: the wordmark reads Agent Running, and the P.S. mark replaces the bridge.

Tradecraft is judgement under uncertainty. The design should feel the same: plain, exact, a little old-fashioned, with nothing decorative that has not earned its place.

## Names

- Set the masthead as **Agent Running**, in `wordmark`, `international-orange`.
- The icon is the **P.S. mark**: the letters "P.S." in `serif` at 600 weight, `on-navy` on a `navy` fill, `radius-md` corners. Use it as the site icon, the social image badge, small (28px) beside Piper's name in each piece's byline, and at the foot of a piece to open the postscript. Meeting it in the byline first teaches readers that P.S. is Piper Smith, so the postscript lands as both. It takes the place the bridge has in the San Francisco Rules. See the PSMark component.
- Refer to the rules as **The San Francisco Rules**, or **SF Rules** after first use. In running text they are Piper's ("my rules"), never a product.
- Piper signs as **P.S.** Set it in `signature`, `navy-text`.

## Voice

- Write in the first person, as Piper. Short sentences. British spelling.
- Write operationally: what I do, what I will not allow, what happens when it goes wrong. No hype, no futurism, no talk of what AI "is".
- End every rule on one line that sticks, set in `closing-line`. Examples from the draft: "If the agent can reset its own counter, the counter is a courtesy." "The agent can pursue the result. It cannot increase the stake."
- Use real operations as evidence: real services, real limits, real numbers (the ZIC checker's 99 attempts). Name them plainly.
- Rules change through use. Mark a rule's status in `label`: DRAFT 2026, REVISED, RETIRED. Never silently rewrite a published rule.
- Never name an intelligence service. Piper's public biography is "Cambridge, Navy, civil service" and nothing more.

## How a rule looks

1. A `label` eyebrow in `orange-text`: RULE 1 · DRAFT 2026.
2. The number in `rule-numeral`, `international-orange`, to the left of the text on wide screens and above it on phones, `space-4` apart.
3. The rule's imperative headline in `rule-title`, ending with a full stop: "Keep the purse outside the operation."
4. The reasoning in `body`, a few short paragraphs.
5. The `closing-line`.
6. Separate rules with `space-5` and a `hairline` divider. Do not box each rule in a card.

Use a `paper-raised` panel for one thing at a time: a quoted field note, an operational figure, or the disclosure.

## Colour

- `paper` is the ground. `ink` is the text. Most of every page is these two.
- `international-orange` is for the wordmark, rule numerals and nothing else large. As text under 24px, use `orange-text`.
- `international-orange` (#c0362c) is the Golden Gate Bridge's own colour. It reads as brick or faded vermilion rather than safety orange; that is intended. The bridge stays in the system as a colour, never as a picture.
- Keep navy. It is Piper's colour and the deliberate second accent; do not fold it into charcoal or orange.
- `navy` and `navy-text` are Piper's: her signature, the P.S. mark, links and the focus ring. Orange speaks for the rules; navy speaks for her.
- Blue and orange stay distinguishable for colour-blind readers. Keep that pairing; do not introduce red and green as a pair.
- `hairline` is decoration only. Anything a reader must notice gets a real colour.
- No gradients. No shadows. No third accent.

## Type

- `display` (Libre Caslon Display) for the wordmark, titles and rule numerals. Never for running text.
- `serif` (Source Serif 4) for everything people read: rule titles, body, closing lines, the signature.
- `mono` (IBM Plex Mono) for labels and operational metadata: dates, file references, allowances, costs. It is the field-report voice. Keep it small but never tiny: labels at 14px, bylines, meta lines and the disclosure at 15px.
- Load all three from Google Fonts. Each family has a system fallback in `type.families`.
- Keep running text near 65 characters a line.

## Layout

- One column of text, left-aligned, with generous `paper` around it. Never centre body copy.
- Masthead at the top: the wordmark, then a single `hairline` rule, then `space-6`.
- On phones the piece title must be the largest text on the page: the wordmark scales down (to 28px) and the title stays at 34px or more.
- Put `space-6` above each section heading in a piece, so a long page on a phone breaks into findable sections.
- Keep a side gutter of at least `space-3` on phones.
- Square corners (`radius-none`) everywhere except controls (`radius-sm`) and the P.S. mark (`radius-md`).

## Imagery

- No Golden Gate Bridge on Agent Running. The bridge belongs to the San Francisco Rules edition; here San Francisco comes through in the colour and the voice.
- No robots, circuit boards, glowing brains or AI symbols. The title and the writing establish the subject.
- If an illustration is needed, draw it in code (SVG), so every line is there because it was specified. No generated images.

## Disclosure

Every page carries this line in its footer, and its page description says the same so search engines and AI agents pick it up:

> Piper Smith is a fictional author created by Charli-Jo Tyrer. Her biography is invented. The operations, ideas and evidence are real.

Set it in `meta`, `ink-muted`, on `paper-raised`.

## Accessibility

- Build to ZIC. Every text pair in this system meets 4.5:1 in both themes; `international-orange` text meets 3:1 and is used only at 24px and above.
- The focus ring is 2px solid `navy-text` with a 2px offset. It reads on `paper` and `paper-raised` in both themes.
- Rule numbers are real text, not images, and each rule is a heading so screen reader users can move rule to rule.
- Both themes are first-class. Light is the archive; dark is the night watch.
