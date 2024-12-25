# Flask Email Verification API

This Flask-based API verifies email addresses by scraping the website "verifyemailaddress.org" using Playwright and BeautifulSoup.

## How it works:
- The API uses Playwright to automate browser interaction.
- After navigating to the verification site, it fills the email input field, clicks the "Verify Email" button, and scrapes the result using BeautifulSoup.
- Returns the verification status in JSON format.

### API Endpoints:
- **`GET /<email>`**: Verifies the given email address and returns the result as a JSON response.

### Example Response:
```json
{
  "response": "Valid email address"
}
