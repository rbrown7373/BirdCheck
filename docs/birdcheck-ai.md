# BirdCheck AI and Voice Questions

BirdCheck AI answers questions about **your saved birding records** and about the bundled **bird catalog**. Open it from **Home → BirdCheck AI**. You can type questions or use iPhone voice input when the relevant feature preference and system permissions are enabled.

## Questions you can try

### Personal history

- “Where was my last outing?”
- “How many birds have I seen in [city]?”
- “What species have I seen in [state]?”
- “How many steps did I take in my last outing?”
- “How far did I walk this week?”
- “Which birds did I see last week?”
- “What birds have I seen in Colorado that I haven't seen in Texas?”

### Catalog questions

- “What birds are in the cardinal family?”
- “Which birds are in [region]?” (A catalog/region question differs from “Which have I seen there?”)

### Follow-up questions

Ask a complete question first, then try “What about last year?” or “How many species is that?” BirdCheck has conversational follow-up handling, but it may clarify when it cannot safely infer a date, region, metric, or comparison.

## Understanding counts

**Distinct species** counts how many different bird identities are supported. **Known recorded individuals** aggregates saved quantities from qualifying dated observations. A Life List-only sighting can count toward species presence without a known individual total.

For a general personal question like “How many birds have I seen in [city]?”, the intended answer gives **both distinct species and known recorded individuals**. If you explicitly ask for species or individuals, BirdCheck should answer that metric.

## Dates and comparisons

“Last week,” “this week,” and “last year” refer to time windows and should use observations with relevant dates. Undated Life List entries should **not** be assigned fabricated observation dates. A two-region set comparison supports **both**, **either**, or **first region excluding the second**, when the question is sufficiently clear. Complex combinations of comparisons and date constraints may require clarification rather than an unreliable answer.

## Important limitations

- BirdCheck AI uses the personal records available **inside the app**. An external assistant reading GitHub documentation **cannot access** those private records.
- Catalog membership is not evidence that you personally saw a species.
- A response about recorded individuals may be incomplete where only undated Life List/location evidence exists.
- Voice transcription is not perfect. If the transcript changes a species or location name, correct the question and retry.
- Questions with genuinely ambiguous places, species names, or comparisons may need clarification.
- AI answers are not a replacement for field identification or scientific verification.

For terminology, see [Data definitions](reference/data-definitions.md). For a support-answering guide, see [AI answering guide](reference/ai-answering-guide.md).
