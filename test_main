from selenium import webdriver
import pytest, time
@pytest.fixture
def browser():
    b = webdriver.Chrome()
    yield b
    b.quit()

def test_example(browser):
    browser.get('http://google.com')
    time.sleep(5)

    assert "Google" == browser.title
