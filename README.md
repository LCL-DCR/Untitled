# Untitled

```python
def search(input):
  try:
  element = WebDriverWait(driver, 10).until (
          EC.presence_of_element_located((By.XPATH, '//*[@id="kpw-header"]/div/div/div/div/form/input'))
      )
      element.send_keys(input)
      element.submit()
      element = WebDriverWait(driver, 10).until (
          EC.presence_of_element_located((By.XPATH, '//*[@id="root"]/div[3]/div/div/div[2]/div[1]/div/a'))
      )
      element.click()
  except:
      driver.quit()
```
