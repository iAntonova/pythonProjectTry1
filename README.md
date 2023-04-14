# pythonProjectTry1

python3 async.py
pytest --headed
pytest --headed --base-url https://www.saucedemo.com --browser webkit --browser chromium --browser firefox
pytest --headed --base-url https://www.saucedemo.com --browser-channel chrome
pytest --headed --base-url https://www.saucedemo.com --device="iPhone 13"

# Tracing:
pytest --headed --base-url https://www.saucedemo.com --browser-channel chrome --tracing on
pytest --headed --base-url https://www.saucedemo.com --browser-channel chrome --tracing retain-on-failure
 -> https://trace.playwright.dev/
or: >  playwright show-trace test-results/pytest-test-saucedemo-py-test-inventory-chromium/trace.zip

# Test generator:
playwright codegen URL

Emulation: https://playwright.dev/python/docs/codegen#emulation
playwright codegen --device="iPhone 13" https://www.saucedemo.com
playwright codegen --viewport-size=800,600 https://www.saucedemo.com
playwright codegen --color-scheme=dark https://www.twitter.com

# Emulate geolocation, language and timezone: https://playwright.dev/python/docs/codegen#emulate-geolocation-language-and-timezone
playwright codegen --timezone="Europe/Rome" --geolocation="41.890221,12.492348" --lang="it-IT" google.com

# Debugging Tests (Playwright Inspector): https://playwright.dev/python/docs/debug
Debugging Selectors: https://playwright.dev/python/docs/debug-selectors

# BrowserContext: https://playwright.dev/python/docs/api/class-browsercontext

# API testing: https://playwright.dev/python/docs/api-testing
# APIRequestContext: https://playwright.dev/python/docs/api/class-apirequestcontext
# Page object models: https://playwright.dev/python/docs/pom
