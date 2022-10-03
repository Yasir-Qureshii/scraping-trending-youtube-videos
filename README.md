## Go to our repo directory

``` Bash
cd remote_control_page/
bash build.sh
```

- Wait for complete building the docker image

```Bash
cd ..
bash setup.sh
```

## Selenium Hub web server
- Check [http://localhost:4444]()
- At this page, you can see we have 5 container web drivers.

![alt text](./assets/selenium_hub.png)
## Remote Control Page
- Check [http://localhost:8050]()

- You can choose your "Facebook Page" and "Proxy" to open new Selenium Driver

- After you "Submit" and "Refresh" you will see web drivers running

![alt text](./assets/1_progress.png)

- Check the port in the view_url field

![alt text](./assets/see_browser.png)

- Then Go to: [http://localhost:7903]() (If you are running locally) or [http://selenium-hub:7903]() (If you are deploying to vm) to see the progress scraping of the web driver 

- Then click "Connect" and Type "secret" for password

![alt text](./assets/web_driver_view.png)

- Finally, you will see the browser running

![alt text](./assets/browser_running_example.png)

- You can also manage all drivers on: [http://localhost:4444/ui#/sessions]()

![alt text](./assets/selenium_hub_session.png)

## Stop the docker containers
```Bash
bash stop.sh
```
