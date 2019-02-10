# Asyncio: We Did It Wrong

Speaker: Lynn Root

Blog post about talk: https://www.roguelynn.com/words/asyncio-we-did-it-wrong/

Initial setup tips... be defensive

* don't accientally swallow exceptions; be sure to "retrieve" them
* Clean up after yourself - loop.close()

asynci.create_task(msg)

await queue.put(msg)


graceful shutdown: tl;dr

* try/except/finally isn't enough
* define desired shutdown behavior
* Use signal handlers
* Listen for appropriate signals

mixing with non-a

* ThreadPoolerExecuter: calling sync from a corout
* create_taks calling a corouting from syanc



https://www.roguelynn.com/words/asyncio-we-did-it-wrong/


