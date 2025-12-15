# IRT Standard for ATProto

A decentralized standard for recording and analyzing test responses using the AT Protocol.

## Overview
This standard enables federated test results and adaptive learning, without exposing question content or violating copyright.

## Lexicon
The lexicon defines the data model and API for the IRT standard.

### Records
- `Test`: Metadata for a test.
- `Question`: Reference to a question (content not federated).
- `Response`: User's response to a question.

### Endpoints
- `createTest`: Create a new test.
- `recordResponse`: Record a user's response.
- `getResponses`: Retrieve responses for analysis.

## Example Usage
```json
{
  "test": {
    "id": "at://irt.example.com/test/123",
    "title": "Math Quiz",
    "description": "Basic algebra questions.",
    "tags": ["math", "algebra"]
  }
}
