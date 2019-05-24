# jq_tutorial_samples

Some samples and commands to parse JSON data.

Let's say the data format is this as shown below :

		{
		  "status": "ok",
		  "totalResults": 38,
		  "articles": [
		    {
		      "source": {
		        "id": null,
		        "name": "Thewire.in"
		      },
		      "author": null,
		      "title": "Arun Jaitley May Not Continue as Finance Minister in New Modi Cabinet - The Wire",
		      "description": "\"He is definitely not taking the post of the finance minister simply because he is very unwell,\" one of the sources, who did not want to be named, told Reuters.",
		      "url": "https://thewire.in/government/arun-jaitley-unlikely-to-continue-as-finance-minister-in-new-modi-cabinet",
		      "urlToImage": "https://cdn.thewire.in/wp-content/uploads/2019/04/04115138/jaitley1_pti-800x400.jpg",
		      "publishedAt": "2019-05-24T10:48:36Z",
		      "content": "New Delhi: Finance Minister Arun Jaitley is unlikely to continue in his current role due to poor health as Prime Minister Narendra Modi begins his second term, according to four sources with knowledge of the matter.\r\nThe sources said that Jaitley, 66, is unli… [+2997 chars]"
		    },
		    {
		      "source": {
		        "id": null,
		        "name": "Sentinelassam.com"
		      },
		      "author": "Poonam Kaur",
		      "title": "Daily Self-Weighing May Help Cut Holiday Weight Gain - The Sentinel Assam",
		      "description": "If you want to avoid adding extra kilos during holidays, engaging in daily self-weighing may help, according to a new research. Previous research has",
		      "url": "https://www.sentinelassam.com/news/daily-self-weighing-may-help-cut-holiday-weight-gain/",
		      "urlToImage": "https://cdn-30-skcir4i63ajp.netdna-ssl.com/wp-content/uploads/2019/05/Weight-Gain.jpg",
		      "publishedAt": "2019-05-24T10:31:27Z",
		      "content": "New York: If you want to avoid adding extra kilos during holidays, engaging in daily self-weighing may help, according to a new research. Previous research has shown the holiday season can lead to weight gain and that persists after end of holidays and could … [+1228 chars]"
		    },
		    {
		      "source": {
		        "id": null,
		        "name": "Firstpost.com"
		      },
		      "author": null,
		      "title": "Lok Sabha Election Results 2019 WINNERS LIVE Updates: BJP makes remarkable comeback in Chhattisgarh after Assembly polls, bags seven out of 11 LS seats - Firstpost",
		      "description": "Lok Sabha election result 2019 WINNERS LIVE updates: Putting behind its debacle in the Assembly elections held just six months ago, the BJP staged a remarkable comeback in Chhattisgarh in the Lok Sabha polls, winning nine of the 11 seats at stake. Watch LIVE …",
		      "url": "https://www.firstpost.com/politics/lok-sabha-election-results-2019-winners-live-updates-bjp-makes-remarkable-comeback-in-chhattisgarh-after-assembly-polls-bags-seven-out-of-11-ls-seats-6688591.html",
		      "urlToImage": "https://images.firstpost.com/wp-content/uploads/2018/11/BJP_Congress_symbols_Reuters2.jpg",
		      "publishedAt": "2019-05-24T10:28:34Z",
		      "content": "Lok Sabha election result 2019 WINNERS LATEST updates: Putting behind its debacle in the Assembly elections held just six months ago, the BJP staged a remarkable comeback in Chhattisgarh in the Lok Sabha polls, winning nine of the 11 seats at stake.\r\nBhojpuri… [+5239 chars]"
		    },
		    {
		      "source": {
		        "id": null,
		        "name": "Ndtv.com"
		      },
		      "author": null,
		      "title": "Election Results 2019: Fallout After Congress Crash - Rash Of Resignations To Rahul Gandhi - NDTV News",
		      "description": "Election results 2019: A day after the Congress's second straight defeat in the national election, resignations were flying. Three state chiefs including Raj Babbar, the Congress's Uttar Pradesh president, sent their resignations to their boss Rahul Gandhi on…",
		      "url": "https://www.ndtv.com/india-news/lok-sabha-election-results-2019-raj-babbar-up-congress-chief-sends-resignation-to-rahul-gandhi-after-2042377",
		      "urlToImage": "https://c.ndtvimg.com/2019-05/dtl5q2mg_raj-babbar-650_650x400_24_May_19.jpg",
		      "publishedAt": "2019-05-24T09:54:00Z",
		      "content": "Election results 2019: Raj Babbar sent his resignation to Rahul Gandhi after Uttar Pradesh defeatNew Delhi: A day after the Congress's second straight defeat in the national election, resignations were flying. Three state chiefs including Raj Babbar, the Cong… [+1866 chars]"
		    },
		    {
		      "source": {
		        "id": "the-times-of-india",
		        "name": "The Times of India"
		      },
		      "author": "Reuters",
		      "title": "Theresa May to step down as British PM on June 7 - Economic Times",
		      "description": "New British PM may be picked within few weeks, says May.",
		      "url": "https://economictimes.indiatimes.com/news/international/world-news/theresa-may-to-step-down-as-british-pm-on-june-7/articleshow/69479621.cms",
		      "urlToImage": "https://img.etimg.com/thumb/msid-69479610,width-1070,height-580,imgsize-43823,overlay-economictimes/photo.jpg",
		      "publishedAt": "2019-05-24T09:52:00Z",
		      "content": "British Prime Minister Theresa May said on Friday she would quit, triggering a contest that will bring a new leader to power who is likely to push for a more decisive Brexit divorce deal.\r\nMay set out a timetable for her departure - she will resign as Conserv… [+1588 chars]"
		    },
		    {
		      "source": {
		        "id": null,
		        "name": "Business-standard.com"
		      },
		      "author": "ANI",
		      "title": "Researchers find hormonal link between diet and obesity - Business Standard",
		      "description": "In a new study researchers have found that low levels of a circulating hormone called adropin predict increased weight gain and metabolic dysregulation during consumption of a high-sugar diet in a nonhuman primate model.According to the study",
		      "url": "https://www.business-standard.com/article/news-ani/researchers-find-hormonal-link-between-diet-and-obesity-119052400827_1.html",
		      "urlToImage": "https://bsmedia.business-standard.com/_media/bs/img/article/default/1190524/full-119052400827.jpg",
		      "publishedAt": "2019-05-24T09:48:45Z",
		      "content": "In a new study researchers have found that low levels of a circulating hormone called adropin predict increased weight gain and metabolic dysregulation during consumption of a high-sugar diet in a nonhuman primate model.\r\nAccording to the study published in t… [+3019 chars]"
		    },
		    {
		      "source": {
		        "id": null,
		        "name": "Hindustantimes.com"
		      },
		      "author": "HT Correspondent",
		      "title": "Prime Minister Narendra Modi gets congratulatory message from India captain Virat Kohli - Hindustan Times",
		      "description": "Apart from Kohli, many cricketers and other sports personalities have also extended their congratulatory messages to PM Modi, who is now set to start his second term as PM.",
		      "url": "https://www.hindustantimes.com/cricket/prime-minister-narendra-modi-gets-congratulatory-message-from-india-captain-virat-kohli/story-ExYbTicVNy04CtWP0z9t7J.html",
		      "urlToImage": "https://www.hindustantimes.com/rf/image_size_960x540/HT/p2/2019/05/24/Pictures/_815d1bcc-7e07-11e9-8a88-8b84fe2ad6da.JPG",
		      "publishedAt": "2019-05-24T09:43:00Z",
		      "content": "Indian captain Virat Kohli might be in England, looking to bring back the World Cup home, but the importance of the political situation back home is not lost upon him. Reacting to the massive victory of Bharatiya Janata Party in the parliamentary elections, K… [+2157 chars]"
		    },
		    {
		      "source": {
		        "id": "the-times-of-india",
		        "name": "The Times of India"
		      },
		      "author": "TNN",
		      "title": "‘Kabir Singh’ first song: ‘Bekhayali’ featuring Shahid Kapoor and Kiara Advani will tug at your heartstri - Times of India",
		      "description": "After impressing the audience with the trailer of the film, the makers of Shahid Kapoor and Kiara Advani starrer, ‘",
		      "url": "https://timesofindia.indiatimes.com/entertainment/hindi/bollywood/news/kabir-singh-first-song-bekhayali-featuring-shahid-kapoor-and-kiara-advani-will-tug-at-your-heartstrings/articleshow/69480034.cms",
		      "urlToImage": "https://static.toiimg.com/photo/msid-69480034/69480034.jpg?458367",
		      "publishedAt": "2019-05-24T09:31:28Z",
		      "content": null
		    },
		    {
		      "source": {
		        "id": null,
		        "name": "News18.com"
		      },
		      "author": "Raka Mukherjee",
		      "title": "Smriti Irani Celebrates Amethi Victory in the Most ‘Game of Thrones’ Way Possible - News18",
		      "description": "After her victory, where she beat Gandhi by  a margin of over 55,000 votes, she took to Instagram to post the Game of Thrones quote on her Instagram.",
		      "url": "https://www.news18.com/news/buzz/smriti-irani-celebrates-amethi-victory-in-the-most-game-of-thrones-way-possible-2157585.html",
		      "urlToImage": "https://images.news18.com/ibnlive/uploads/2019/05/Untitled-design-317.png",
		      "publishedAt": "2019-05-24T09:29:50Z",
		      "content": "This month saw two battles: The Battle for the Iron Throne on Game of Thrones, and in India, the Lok Sabha Elections.'The North remembers' is a pretty common phrase used in Game of Thrones, and if you've watched the show, you'll know exactly what it means. Fo… [+2490 chars]"
		    },
		    {
		      "source": {
		        "id": null,
		        "name": "Icc-cricket.com"
		      },
		      "author": "ICC",
		      "title": "India, New Zealand seek tune-up in warm-up clash - International Cricket Council",
		      "description": "The Indian team, led by Virat Kohli will take on Kane Williamson's New Zealand at The Oval on Saturday, aiming to find answers to their ideal playing combinations ahead of the ICC Men's Cricket World Cup 2019.",
		      "url": "https://www.icc-cricket.com/news/1225448",
		      "urlToImage": "https://resources.pulse.icc-cricket.com/ICC/photo/2019/05/24/6e57c5f8-ab23-4c4c-a7c8-e2d7d1cb2b7b/Lead.jpg",
		      "publishedAt": "2019-05-24T09:24:41Z",
		      "content": "The Indian team, led by Virat Kohli will take on Kane Williamson's New Zealand at The Oval on Saturday, aiming to find answers to their ideal playing combinations ahead of the ICC Men's Cricket World Cup 2019.Overview\r\nIndia v New Zealand\r\nThe Oval, London201… [+3691 chars]"
		    },
		    {
		      "source": {
		        "id": null,
		        "name": "News18.com"
		      },
		      "author": "News18.com",
		      "title": "PM Narendra Modi Biopic Reviews: Critics Call it a Hagiography, Vivek Oberoi's Acting Panned - News18",
		      "description": "While we await the movie's box office fate, critics have already passed their verdict on the biopic PM Narendra Modi.",
		      "url": "https://www.news18.com/news/movies/pm-narendra-modi-biopic-reviews-critics-call-it-a-hagiography-vivek-oberois-acting-panned-2157687.html",
		      "urlToImage": "https://images.news18.com/ibnlive/uploads/2019/05/PM-Narendra-Modi-biopic_poster-vivek-oberoi.jpg",
		      "publishedAt": "2019-05-24T09:01:07Z",
		      "content": "PM Narendra Modi, the biopic on the prime minister which has Vivek Oberoi playing the titular role, finally saw the light of day today. The film's release was stalled after the Election Commission placed a ban on it in order to follow model code of conduct. T… [+2700 chars]"
		    },
		    {
		      "source": {
		        "id": null,
		        "name": "Gsmarena.com"
		      },
		      "author": "Ro",
		      "title": "Redmi 7A announced with Snapdragon 439 and 4,000 mAh battery - GSMArena.com news - GSMArena.com",
		      "description": "It also comes with P2i water-repellent nanocoating.",
		      "url": "https://www.gsmarena.com/redmi_7a_announced_with_snapdragon_439_and_4000_mah_battery-news-37206.php",
		      "urlToImage": "https://cdn.gsmarena.com/imgroot/news/19/05/redmi-7a-offic/-476x249w4/gsmarena_000.jpg",
		      "publishedAt": "2019-05-24T08:40:01Z",
		      "content": "Xiaomi's Redmi brand just announced its most affordable smartphone from the series - the Redmi 7A. The handset is a direct successor to the Redmi 6A and packs a couple of hard to find features for the asking price.\r\nFor starters, the phone runs on a Snapdrago… [+1013 chars]"
		    },
		    {
		      "source": {
		        "id": "the-times-of-india",
		        "name": "The Times of India"
		      },
		      "author": "PTI",
		      "title": "BSP biggest gainer among mahagathbandan constituents in UP - Economic Times",
		      "description": "After drawing a blank in the 2014 general election, the Bahujan Samaj Party this time round won a decent 10 of the 38 seats that it contested as part of the alliance in Uttar Pradesh.",
		      "url": "https://economictimes.indiatimes.com/news/elections/lok-sabha/uttar-pradesh/bsp-biggest-gainer-among-mahagathbandan-constituents-in-up/articleshow/69478745.cms",
		      "urlToImage": "https://img.etimg.com/thumb/msid-69478739,width-1070,height-580,imgsize-606181,overlay-economictimes/photo.jpg",
		      "publishedAt": "2019-05-24T08:40:00Z",
		      "content": "The performance of the BSP-SP-RLD mahagathbandhan might have fallen short of expectations and also shattered her prime ministerial aspirations, but BSP supremo Mayawati has been a major gainer in the 2019 Lok Sabha elections.\r\nAfter drawing a blank in the 201… [+1963 chars]"
		    },
		    {
		      "source": {
		        "id": "the-times-of-india",
		        "name": "The Times of India"
		      },
		      "author": null,
		      "title": "Lok Sabha election results: Narendra Modi, the PM who is more like a President - ​Modi ran a tight ship with firmness - Economic Times",
		      "description": "In his first term, Narendra Modi ran a tight ship with a firmness that no Indian Prime Minister has been able to exercise since Indira Gandhi.His control over the government was total, akin to the hold US presidents have over their team, or the type of clout …",
		      "url": "https://economictimes.indiatimes.com/news/elections/lok-sabha/india/lok-sabha-election-results-narendra-modi-the-pm-who-is-more-like-a-president/modi-ran-a-tight-ship-with-firmness/slideshow/69478601.cms",
		      "urlToImage": "https://img.etimg.com/thumb/msid-69478601,width-1070,height-580,overlay-economictimes/photo.jpg",
		      "publishedAt": "2019-05-24T08:30:00Z",
		      "content": "Both the Shiv Sena and JD(U) have been remorseless in setting the cost of their support. The veracity of the speculation that TRS chief K Chandrasekhar Rao, sniffing the prospect of a hung house, had started scouting for support for his aspiration to be deput… [+616 chars]"
		    },
		    {
		      "source": {
		        "id": null,
		        "name": "Ndtv.com"
		      },
		      "author": null,
		      "title": "2 Indians Among 3 Dead As 'Traffic Jam' On Everest Puts Climbers At Risk - NDTV News",
		      "description": "Three more climbers have died on Everest, expedition organisers and officials said Friday, taking the toll from a deadly week on the overcrowded peak of the world's tallest mountain to seven.",
		      "url": "https://www.ndtv.com/world-news/three-more-die-on-overcrowded-mount-everest-death-toll-reaches-7-2042360",
		      "urlToImage": "https://c.ndtvimg.com/2019-05/h3sneg4_everest-_625x300_24_May_19.jpg",
		      "publishedAt": "2019-05-24T08:25:00Z",
		      "content": "A huge queue of climbers formed near the summit of Mount Everest on Thursday. (File)Kathmandu: Three more climbers have died on Everest, expedition organisers and officials said Friday, taking the toll from a deadly week on the overcrowded peak of the world's… [+3065 chars]"
		    },
		    {
		      "source": {
		        "id": null,
		        "name": "Ndtv.com"
		      },
		      "author": null,
		      "title": "Key Things To Know About SBI's Basic Savings Bank Deposit Account - NDTV News",
		      "description": "SBI's zero balance account: A basic RuPay ATM-cum-debit card is issued free of cost and no annual maintenance charge is applied. The receipt/ credit of money through electronic payment channels like NEFT/RTGS is free. The deposit/ collection of cheques drawn …",
		      "url": "https://www.ndtv.com/business/state-bank-of-india-sbi-zero-balance-account-basic-savings-bank-deposit-bsbd-account-interest-rates-2042417",
		      "urlToImage": "https://i.ndtvimg.com/i/2018-03/state-bank-of-india-sbi_650x400_51520955294.jpg",
		      "publishedAt": "2019-05-24T08:07:00Z",
		      "content": "Zero balance account in SBI: BSBD account can be opened by any individual by taking up KYC verification.State Bank of India (SBI) offers a special type of savings bank account, known as the basic savings bank deposit or BSBD account. A zero balance savings ac… [+2438 chars]"
		    },
		    {
		      "source": {
		        "id": null,
		        "name": "Indiatoday.in"
		      },
		      "author": null,
		      "title": "India's Most Wanted Movie Review: Arjun Kapoor leads a manhunt in tepid thriller - India Today",
		      "description": "Arjun Kapoor sets out with his team of ordinary faceless men to hunt India's Most Wanted man. The film deserves a watch for its second half.",
		      "url": "https://www.indiatoday.in/movies/bollywood/story/india-s-most-wanted-movie-review-arjun-kapoor-leads-a-manhunt-in-tepid-thriller-1533586-2019-05-24",
		      "urlToImage": "https://akm-img-a-in.tosshub.com/indiatoday/images/story/201905/indias-most-wanted-review-647x363.jpeg?eUJJU6hn0LNQPdJIDJoUIb2f0I0YFheI",
		      "publishedAt": "2019-05-24T07:36:00Z",
		      "content": null
		    },
		    {
		      "source": {
		        "id": null,
		        "name": "Ndtv.com"
		      },
		      "author": null,
		      "title": "Election Results 2019: A Sweet And Sour Win For DMK Chief MK Stalin - NDTV News",
		      "description": "It's a sweet and sour victory for the DMK which has swept Tamil Nadu in the national elections. Party chief MK Stalin, who faced his first major electoral test after his father and party patriarch M Karunanidhi's death last year, proved his leadership deliver…",
		      "url": "https://www.ndtv.com/india-news/election-results-2019-a-sweet-and-sour-win-for-dmk-chief-mk-stalin-2042283",
		      "urlToImage": "https://c.ndtvimg.com/2019-05/hu6skhq_mk-stalin_625x300_24_May_19.jpeg",
		      "publishedAt": "2019-05-24T07:27:00Z",
		      "content": "DMK chief MK Stalin thanked the people of Tamil Nadu for \"resounding victory\".Chennai: It's a sweet and sour victory for the DMK which has swept Tamil Nadu in the national elections. Party chief MK Stalin, who faced his first major electoral test after his fa… [+3631 chars]"
		    },
		    {
		      "source": {
		        "id": null,
		        "name": "Hindustantimes.com"
		      },
		      "author": "HT Correspondent",
		      "title": "Katrina Kaif asks Salman Khan why he doesn’t follow her on Instagram, his answer is hilarious - Hindustan Times",
		      "description": "Katrina Kaif was in her elements as she promotes her new film Bharat with Salman Khan.",
		      "url": "https://www.hindustantimes.com/bollywood/katrina-kaif-asks-salman-khan-why-he-doesn-t-follow-her-on-instagram-his-answer-is-hilarious/story-YPcWo3n2VV3CNZFIlZOu5I.html",
		      "urlToImage": "https://www.hindustantimes.com/rf/image_size_960x540/HT/p2/2019/05/24/Pictures/_f14b4e96-7ded-11e9-8a88-8b84fe2ad6da.jpg",
		      "publishedAt": "2019-05-24T07:10:00Z",
		      "content": "Actor Katrina Kaif has been busy promoting her next film Bharat, where she stars with Salman Khan. Katrina, who is close friends with her co-actor too, rarely loses a chance to pull his leg. At a recent media interaction, Katrina was reminded of her comment t… [+2152 chars]"
		    },
		    {
		      "source": {
		        "id": null,
		        "name": "Expresshealthcare.in"
		      },
		      "author": "EH News Bureau",
		      "title": "Unhealthy food at work may up risk of lifestyle ailments: Study - Express Healthcare",
		      "description": "Research has shown obesity contributes to higher absenteeism, lower productivity and higher healthcare expenses for employers",
		      "url": "https://www.expresshealthcare.in/news/unhealthy-food-at-work-may-up-risk-of-lifestyle-ailments-study/411670/",
		      "urlToImage": "https://cdn.expresshealthcare.in/wp-content/uploads/2016/07/28063838/Obesity-Re.jpg",
		      "publishedAt": "2019-05-24T06:54:23Z",
		      "content": "Research has shown obesity contributes to higher absenteeism, lower productivity and higher healthcare expenses for employers\r\nEmployees who purchase unhealthy food at office may indulge in such diet outside work as well, increasing their risk of lifestyle ai… [+2579 chars]"
		    }
		  ]
		}

To get the first paragraph

		$cat news.json|jq '.articles[0]'
		{
		  "source": {
		    "id": null,
		    "name": "Thewire.in"
		  },
		  "author": null,
		  "title": "Arun Jaitley May Not Continue as Finance Minister in New Modi Cabinet - The Wire",
		  "description": "\"He is definitely not taking the post of the finance minister simply because he is very unwell,\" one of the sources, who did not want to be named, told Reuters.",
		  "url": "https://thewire.in/government/arun-jaitley-unlikely-to-continue-as-finance-minister-in-new-modi-cabinet",
		  "urlToImage": "https://cdn.thewire.in/wp-content/uploads/2019/04/04115138/jaitley1_pti-800x400.jpg",
		  "publishedAt": "2019-05-24T10:48:36Z",
		  "content": "New Delhi: Finance Minister Arun Jaitley is unlikely to continue in his current role due to poor health as Prime Minister Narendra Modi begins his second term, according to four sources with knowledge of the matter.\r\nThe sources said that Jaitley, 66, is unli… [+2997 chars]"
		}


To get the second paragraph

	$  cat news.json |jq '.articles[1]'

		{
		  "source": {
		    "id": null,
		    "name": "Sentinelassam.com"
		  },
		  "author": "Poonam Kaur",
		  "title": "Daily Self-Weighing May Help Cut Holiday Weight Gain - The Sentinel Assam",
		  "description": "If you want to avoid adding extra kilos during holidays, engaging in daily self-weighing may help, according to a new research. Previous research has",
		  "url": "https://www.sentinelassam.com/news/daily-self-weighing-may-help-cut-holiday-weight-gain/",
		  "urlToImage": "https://cdn-30-skcir4i63ajp.netdna-ssl.com/wp-content/uploads/2019/05/Weight-Gain.jpg",
		  "publishedAt": "2019-05-24T10:31:27Z",
		  "content": "New York: If you want to avoid adding extra kilos during holidays, engaging in daily self-weighing may help, according to a new research. Previous research has shown the holiday season can lead to weight gain and that persists after end of holidays and could … [+1228 chars]"

		}



To get the author of the first paragraph


	$ cat news.json |jq '.articles[1].author'
	"Poonam Kaur"


To get the title of the first paragraph

	$ cat news.json |jq '.articles[1].title'
	"Daily Self-Weighing May Help Cut Holiday Weight Gain - The Sentinel Assam"


To get the length of different paragraphs

	$ cat news.json |jq '.[] |length'
	2
	38
	20

To get all the titles 


