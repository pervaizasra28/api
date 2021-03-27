# api
working with api's
url = "https://newsapi.org/v2/everything" 
myAPIkey = "2a0b727b2220426298fa6cc9d2c3ded1"
article = {'q' : 'Everything' + myAPIkey}
params = {
    "q"  : "Covid" ,
    "apikey" : "2a0b727b2220426298fa6cc9d2c3ded1"
}

resp = requests.get(url , params = params)
data = resp.json()
data

new_url = "https://newsapi.org/v2/everything?domains=cnn.com,bbc.com,thenextweb.com&apiKey=2a0b727b2220426298fa6cc9d2c3ded1"
requests.get(new_url).json()

requests.get(new_url).json()
sources = 'https://newsapi.org/v2/sources?apiKey=2a0b727b2220426298fa6cc9d2c3ded1'
params = {
    'language' : 'en'
}
resp = requests.get(sources, params = params)
resp.json()
