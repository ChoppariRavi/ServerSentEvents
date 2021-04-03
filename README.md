# ServerSentEvents


EventSource
The EventSource interface is web content's interface to server-sent events. An EventSource instance opens a persistent connection to an HTTP server, which sends events in text/event-stream format. The connection remains open until closed by calling EventSource.close().

**cd sse-server**<br/>
**node server.js**<br/>
**Output**<br/>
**Facts Events service listening at http://localhost:3001**

**cd sse-client**<br/>
**npm start**


```curl -X POST \
 -H "Content-Type: application/json" \
 -d '{"info": "Shark teeth are embedded in the gums rather than directly affixed to the jaw, and are constantly replaced throughout life.", "source": "https://en.wikipedia.org/wiki/Shark"}'\
 -s http://localhost:3001/fact```
