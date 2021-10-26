#I-Tunes API: 
import requests
site= "https://itunes.apple.com/search"
url = site+"/?term=the+beatles&country=us"
requests.get(url)

r=requests.get(site, params= {"term": "the beatles", "country": "us" } )
#print(r.status_code) # correctly prints 200

info=r.json()
print(info.keys() )
print(info['results'])

--------------------------

#  https://official-joke-api.appspot.com/random_joke
import requests
site2="https://official-joke-api.appspot.com/random_joke"
r=requests.get(site2)
info=r.json()
# print(info.keys()) # dict_keys(['id', 'type', 'setup', 'punchline'])
id1=info['id']
type1=info['type']
setup=info['setup']
line=info['punchline']
print(id1, type1, setup, line)



-----------------------------

#This was an API challenge given to me by a friend:
# https://api.coingecko.com/api/v3/coins
import requests
site3="https://api.coingecko.com/api/v3/coins"
r=requests.get(site3)
#print(r.status_code) #correctly prints 200

info=r.json()
id1=info[0]['id']
keys=info[0].keys()
#print(keys) #dict_keys(['id', 'symbol', 'name', 'block_time_in_minutes', 'image', 'market_data', 'last_updated', 'localization'])
price=info[0]['market_data']['current_price']['usd'] #gets the price 
for i in range( len(info) ):
    print( info[i]['name']   )
    print( info[i]['market_data']['current_price']['usd']   )
print("Done")


#for key,value in price.items():
    #print("Key : {} , Value : {}".format(key,value))
#print(id1, price)
#print(r.keys() )
