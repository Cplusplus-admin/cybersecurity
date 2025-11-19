# 🟢 what's mine is yours

first unintended way

<figure><img src="../../../../.gitbook/assets/image (20).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/image (21).png" alt=""><figcaption></figcaption></figure>

very simple looking website which has only sign in button so we will do the usual test functionality and see where it goes

<figure><img src="../../../../.gitbook/assets/image (22).png" alt=""><figcaption></figcaption></figure>

one click made 3 request we will analyze all the 3 one by one

<figure><img src="../../../../.gitbook/assets/image (23).png" alt=""><figcaption></figcaption></figure>

it set's cookie

<figure><img src="../../../../.gitbook/assets/image (24).png" alt=""><figcaption></figcaption></figure>

it sets cookie in next request

<figure><img src="../../../../.gitbook/assets/image (25).png" alt=""><figcaption></figcaption></figure>

got api token and as the chall says we will go to `/api/flag` and put this api token in `X-Flag-Token`

<figure><img src="../../../../.gitbook/assets/image (26).png" alt=""><figcaption></figcaption></figure>

it says not found&#x20;

next i decided to change request methods because in response headers of  `/login` request it says access control allow methods GET, POST, OPTIONS and i without any thought behind it tried it

<figure><img src="../../../../.gitbook/assets/image (27).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/image (28).png" alt=""><figcaption></figcaption></figure>

very interesting error just because i changed method of request

so i added cookie from our session as it say 'not authenticated'

<figure><img src="../../../../.gitbook/assets/image (29).png" alt=""><figcaption></figcaption></figure>

i don't know how but it worked

my real intention was changing method to see if there's any different outcome and yes it did but i didn't expect i was on my way to flag but when i put my own cookie because it said 'not authenticated' and gave 401 unauthorized error flag shouldn't have revealed, i tried this challenge 2 times(my first try and 2nd try while posting this challenge) with different cookies and token result was same.
