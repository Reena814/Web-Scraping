result, continuation_token = reviews(
   'com.ubercab.eats',
   lang='en',
   country='us', 
   sort=Sort.NEWEST, 
   count=10000,
)
result, _ = reviews(
   'com.ubercab.eats',
   continuation_token=continuation_token
)
