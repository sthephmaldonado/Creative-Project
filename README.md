# Creative-Project

### Summary 
For this Creative Project I decided to make it out of two philosophical texts “The Little Prince” by Antoine de Saint-Exupéry and “The Prophet” by Kahlil Gibran. 

The little prince tells the story of a pilot who, while trying to repair his damaged plane in the middle of the Sahara Desert, runs into a little prince from asteroid B 612.
A flower grew on the floor of the asteroid of the little prince. The little prince tries to take care of it, but the flower was capricious. The little prince abandons his asteroid and embarks on a journey through the universe in search of a friend. On the journey, the little prince visits several asteroids until he reaches Earth, he met a varied group of eccentric characters who convince him of how strange the world of adults is, always so busy with serious and important matters, that they forget to enjoy life.
On Earth, the little prince came into contact with animals, flowers and people. It was there where he meets the fox, who will reveal to him the importance of friendship and the value of the love he feels for his flower. It will be the nostalgia for her (flower) and the disappointment that the adult world causes him that will motivate the little prince to return to his planet.

The Prophet is written as a short prose poem that tries to encourage the reader to change their way of life based mainly on leading it in a balanced way with respect to divinity and inner peace. For Gibran, the obstacles and vicissitudes of the world are only tests that allow man to evolve and advance on the path towards purification, thus he shows us that the world will be better when men are able to come closer and coexist. Through his phrases, the understanding of numerous human emotions, temptations and feelings, such as pleasure, money, love, death and marriage is reached.

These two texts give life lessons, and they employ a fairly simple narrative style. One can be considered a children's book because of the way it is written but in which deep issues are actually addressed. In my opinion the combination of the texts will be generating an interesting text, since both texts a really philosophical oriented, focused on different aspects of life and how those can be addressed. Having an end result of a text that can deeply help or advice in some way on how to live life. 

### Steps creating the text

1.	Using Markovify
•	I combined both texts into one single txt file (PrinceProphet.txt). 
•	Then I used Exercise 1 as reference
•	Run all the cells and adding my txt (PrinceProphet.txt)
•	Generating my new Markovify text 
2.	GPT-2 
•	Create a copy of train a GTP-2 text-generating model w/GPU
•	Run each cell and add my new Markovify text
o	Before reaching the “Generate Text From The Trained Model” section the code was changed 
gpt2.generate(sess,
              length=750,
              temperature=0.5,
              prefix="The secret to live life",
              nsamples=5,
              batch_size=5
              )
o	Length to 750 to create the 3000 words required 
o	Temperature 0.5 to keep the text neutral 
o	Prefix so each returned text can start with a “secret”

I would like to comment that the GPT-2 part took too much time; it took me almost 3 days to generate the ending text. I tried terminating all my sessions, creating new files and running everything again, but I didn’t have any success, after trying and trying I opened a new copy of GPT (at night I am not sure if this influence in something) changed to safari instead of chrome and it worked, it generated a text (text below). I wanted to keep everything in one single notebook, but I just couldn’t, it never finished training. I will keep trying and if I come up with any results, I will update this part. 

### How to run the Project
1.	Open the Creative Project (ipynb) file 
2.	Download and upload Markovify.txt
3.	Run each cell 
4.	On Finetune section wait until its stops training 
5.	Continue running each cell
6.	On the Generated text from the pretrained model section you will get the final results of the text 

### Samples 

**The secret to live life and dance to the song of the city gate and by night they would be revealed to me. I, too, shall look into space; you shall see. And the people as from a slight distance, that would make a stream upon whose bank you would accept the seasons of your beauty, yet they belong not to clear them.Suffer not yet our eyes to hunger for your growth so is he not more sweetly to the wind speaks not more mindful of his pigmy-self and the sun to them but a flash of yellow close to tears.I could not have you sing it with its roots.*

**For in that knowledge become a memory. We wanderers, ever seeking the lonelier way, begin no day where we have given a much greater air of truth to my knees--and one of you would accept the seasons for their steps in the quiet urge that reveals your power?*
The secret to live life without sorrow?It is the captain of my eye, and you are in truth loving life, And to the sea, carrying the secrets of your dreams.And there are also as strong as your weakest link.Then he mopped his forehead with a certain sense of grief?Fain would I have three volcanoes.Your daily life is darkness, and in his life but add up figures.*

**Aye, in the sunlight and the sun is your god-self; It remains for ever undefiled.Yet unless the exchange be in the sand.
And he said: You would measure time into seasons, let each season encircle all the stars will be properly astonished to see all else, And if not the deep nor the high.*

The temperature influenced the text, so I tried to keep it less than 0.7. I wanted to try it on 0.1 but since I was able to train the text just once, I couldn’t go back and play more with the temperature. Unfortunately, I run the cells again because the runtime wasn’t working anymore. So I couldn’t keep working on it nor save it on the notebook, but I actually copy and paste the text that was generated since I saw that coming.  

### Artist Statement 
I managed to work with Markovify and GTP-2. It was really frustrating that training the text took too much time, I could only generate one text of the GPT and it wasn’t in the same notebook I wanted it to be. I think both texts helped on the outcomes of the project, each book has a unique philosophy for life. Even though some results on the text seem off, its impressive that it actually have some that makes sense and are precise on looking answers for “the secret to live life”.
While I was working on it, I thought it would be interesting working more on the project and see if GPT-2 can give any philosophical response to different questions using the already combined and generated text from Markovify. After researching I found some articles that GPT-3 actually does that (https://dailynous.com/2020/07/30/philosophers-gpt-3/) in a future it will intriguing to see the results. 

