# codex-assistant-data

Data repository for Codex Assistant application.

## Structure

- /laws/ - Law files for different servers
- /rules/ - Rules files by category
- epo_structure.json - List of available files
- anner.json - Banner configuration

## Data Format

### Law files
`json
{
  "updatedAt": 1734444000000,
  "data": {
    "UK": {
      "url": "forum link",
      "articles": []
    }
  }
}
{
  "updatedAt": 1734444000000,
  "data": {
    "main-rules": {
      "articles": []
    }
  }
}
