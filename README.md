# linebot-fastapi

## How to run
1. export your `LINE_CHANNEL_ACCESS_TOKEN` and `LINE_CHANNEL_SECRET`

2. run this command in terminal to open server
```bash
uvicorn main:app --host 0.0.0.0 --port 8080 --reload
```

3. run ngrok to open tunnel
```bash
docker run --rm --net=host -it -e <TOKEN> ngrok/ngrok http 8080
```

4. paste the `<ngrok_url>/webhooks/line` in Line Developer (webhook url)
