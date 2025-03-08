# Contributing to Ingot's Game

This is the collection of ingot's game prompts.

I threw in some AI generated prompts to start things off but will probably remove a lot of them, improve the difficulty system and add more creative ones.

## How to Contribute

### 1. Adding New Prompts
- Ensure the prompt is **unique** and not already in the list.
- Pick a difficulty level between **1** (easiest) and **9** (hardest) based on how challenging the prompt is and how many players are left. 

**Important:** The prompt must have **at least** as many valid answers as the number of remaining players. The difficulty level is calculated using the formula:

`(max_players - remaining_players) + 1`, where `max_players = 10`.

This ensures that prompts do not become impossible to answer. 
So prompts having less answers than players alive are BAD prompts (e.g. "how many planets are there in the solar system?" would be invalid when the remaining players are more than 8).

_Note:_ this difficulty system will probably be changed in the future.

- Add the prompt and difficulty in the JSON file using the format:
  
  ```json
  {
    "New prompt category": difficulty_level
  }
  ```
- Example:
  ```json
  {
    "Famous jazz musicians": 4
  }
  ```

### 2. Updating Existing Prompts
- If you think a prompt's difficulty level is incorrect, suggest a change via a **GitHub Issue**.
- If an existing prompt could be reworded for clarity, propose the revision in an issue or pull request.

### 3. Removing Redundant or Incorrect Entries
- If a prompt is **duplicate**, **too broad**, or **factually incorrect**, suggest its removal by opening a **GitHub Issue**.

## Submission Guidelines
1. **Fork** the repository.
2. Make your changes in a new branch.
3. Submit a **pull request (PR)** with a clear description of the changes.
4. Ensure JSON syntax is valid before submitting.
5. Engage in discussions on issues and PRs when needed.

## Contribution Rules
- Keep prompts **concise** and **clear**.
- Avoid highly subjective or ambiguous topics.
- Respect the difficulty scale to maintain consistency.

## Example Prompt List Entry
```json
{
  "Olympic sports": 3,
  "Famous inventors": 5,
  "Historic battles": 7
}
```

