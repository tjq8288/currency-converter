# Security Policy

## Supported Versions

We release patches for security vulnerabilities. Which versions are eligible for receiving such patches depends on the CVSS v3.0 Rating:

| Version | Supported          |
| ------- | ------------------ |
| 1.x.x   | :white_check_mark: |

## Reporting a Vulnerability

The Currency Converter team takes security bugs seriously. We appreciate your efforts to responsibly disclose your findings, and will make every effort to acknowledge your contributions.

To report a security issue, please use the GitHub Security Advisory ["Report a Vulnerability"](https://github.com/tjq8288/currency-converter/security/advisories/new) tab.

The team will send a response indicating the next steps in handling your report. After the initial reply to your report, the security team will keep you informed of the progress towards a fix and full announcement, and may ask for additional information or guidance.

## Security Considerations

This Currency Converter:
- ✅ Runs entirely client-side (no server communication)
- ✅ Does not collect or store personal financial data
- ✅ Uses HTTPS when deployed on GitHub Pages
- ✅ Does not store conversion history locally by default
- ✅ Implements secure API key handling (when applicable)
- ✅ Uses Content Security Policy (CSP) headers

## Privacy & Financial Data

- **No Data Collection**: All conversions are performed locally in your browser
- **No Financial Tracking**: No currency amounts, transaction data, or personal information is stored
- **API Rate Limiting**: External rate requests are throttled to prevent abuse
- **Offline Capable**: Works without internet connection using cached rates
- **No Cookies**: No tracking cookies or persistent session storage used

## Exchange Rate Security

- **Rate Verification**: Multiple source validation for accuracy
- **Tamper Protection**: Client-side rate validation mechanisms
- **Update Frequency**: Regular rate updates to prevent stale data
- **Source Diversity**: Multiple exchange rate providers for redundancy
- **Error Handling**: Graceful degradation when rate services are unavailable

## Financial Security Best Practices

When using any currency converter:
- ✅ Verify rates with multiple sources before large transactions
- ✅ Use official bank rates for actual currency exchanges
- ✅ Never enter sensitive financial account information
- ✅ Be aware that rates shown are for reference only
- ✅ Understand that market rates change constantly
- ✅ Consult financial professionals for major currency decisions

## API Security (If Applicable)

- **Rate Limiting**: API calls are limited to prevent abuse
- **HTTPS Only**: All external API requests use secure connections
- **Key Rotation**: API keys are rotated regularly
- **Error Handling**: No sensitive information leaked in error messages
- **Timeout Protection**: Request timeouts prevent hanging connections
