# python3 async.py
# pytest --headed
# pytest --headed --base-url https://www.saucedemo.com --browser webkit --browser chromium --browser firefox
# pytest --headed --base-url https://www.saucedemo.com --browser-channel chrome
# pytest --headed --base-url https://www.saucedemo.com --device="iPhone 13"
#
# Tracing:
# pytest --headed --base-url https://www.saucedemo.com --browser-channel chrome --tracing on
# pytest --headed --base-url https://www.saucedemo.com --browser-channel chrome --tracing retain-on-failure
#  -> https://trace.playwright.dev/
# or: >  playwright show-trace test-results/pytest-test-saucedemo-py-test-inventory-chromium/trace.zip
#
# Test generator:
# playwright codegen URL