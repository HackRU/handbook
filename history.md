# History

This is just reminiscing, but will give some context. Read if interested.

## Origins

R&D didn't exist before 2016. In November 2016, particularly, the name architect came to exist.
This was probably the first or second R&D thing that happened. Carlin came up with the idea and
explained it to me (Heman). It was inspired by MIT's tech team.

The name architect was probably the hardest R&D tradition that was decided in 2016. There were
many other ideas: "builders," "creators," "designers," or just "organizers" - and then we settled
on "architects." I think it's important to realise [what and architect is](architects.md#what-is-an-architect).
It's odd, since in terms of HackRU's central organization, architects are organizers.

After this, in December and January, we settled on an interview process. The familiar process
was somewhat controversial - HackRU does not interview most organizers, only R&D architects.
Carlin initially suggested that the question merely asked to generate primes.
The question that replaced it was the "contraction contraption."

## The First Wave of R&D

The first R&D email looked like this:

 > Hello there!
 > 
 > Congratulations fellow hacker!  You have passed the first challenge in becoming an Architect for HackRU!  (Actually filling out the form.)  The next step is a quick coding challenge - the contraction contraption - so we can better analyse your skills and thought process. We require that you take less than 3 days (until the end of the coming Wednesday, 1/18) to answer the questions. Please provide us with all the details that you feel are necessary to properly understand and run your code. Note that the first question asks for a runnable implementation while the second asks for a design.
 > 
 > Here are the questions:
 >   1) Write a function that takes a sentence as a string and returns a string with all the contractions instead (ie. "is not" becomes "isn't"). Convert at least [should, could, would, do, is, are, does, have] not => []n't and [should, could, would] have => []'ve. Many may occur in a sentence. Words will be delimited by single spaces and will not contain punctuation.
 >   2) Multiple contractions can be chained in some cases: there's a famous Southern "y'all'd've" (you all would have) which y'all'd'ven't (you all would have not) heard of if y'all'evn't (you all have not (I may be making this one up)) been to the South. Additionally, Scottish slang allows for "am not" to be written as "amn't," which ain't different from "ain't." Design an app to let users input sentences and get shortened (or even expanded) ones back. How would you allow them to conveniently configure your tool to handle all sorts of contractions (even their own, or their own odd chains)?
 > 
 > We hope for this to be rather conversational though in email form. Please let us know if you need any clarifications! We will send follow-up questions and hope you hear from you soon.
 > 
 > Thank you for your interest in HackRU RND and good luck.
 > 
 > Best,
 > Qasim and Heman,
 > Directors, HackRU RND.

The answers varied from tokenisers that read the input word-by-word and slowly built the new sentence by checking the words to
quick and clever hashmap implementations that grabbed words out of a hash map
and replaced with the contraction.

A hidden gem was the string "should have not" which most people made "should've not" but reversing implementations and some
hashing ones made "should haven't". Follow-ups asked about this and big-O as it was decided here that follow-ups would be nice.

The design question was a lot of fun - people discussed NLP, AI, a social media (like a stack exchange site), and various potential
mobile apps.

We were surprised that without much advertisement, we got 20 responses! Furthermore, most people were very, very talented, having
had internships, or researching AI, or just generally having bad-ass githubs. The only travesty was that we did not have any
diversity.

In the last few weeks of January we were ready to meet the architects.

## The First Meetings and Projects

The first few R&D meetings were not that great. Qasim and I did not know what we were doing.
We just kept getting late people and building their confidence without concretely defining the
more difficult projects.

We were really lucky in that Carlin took care of the main website. This became a much larger concern later on.
The projects were:
 - A slackbot (as always)
 - A day-of dashboard
 - Gavel: tweaks to the judging platform
 - QRU: a QR-code based registration system
 - A mobile app: to let QR scanning happen.
 - A photo filter: so people can update their profile pics for HackRU hype.

The photo filter was the first time we coordinated with the marketing team. This is sort of of historical importance: marketing
is the team we talk to the most. [Cong](https://github.com/CongWangStatic) finished this in a few weeks.

The day-of dashboard was a last-minute miracle. It was crashing on the day-of and just about worked, but was very nice.
It was a HackRU first and people were clamouring for it for a while. [Jan](https://github.com/jandeancatarata) did this with surprisingly little oversight,
bringing ReactJS to HackRU for the first time.

The slackbot too suffered on the day-of. However, they were the first R&D team to live on their own: they just managed and delivered
a bot with minimal intervention from the directors. [Sam](https://github.com/Azoam) led the project and was advised by [Sri](https://github.com/Sail338).

QRU and the mobile app were nice. The app was very last minute, but worked. [Steve](https://github.com/bnjw5jhyxn) wrote it in ionic and a crazy Linux set-up and learning a lot on the fly.
[Varun](https://github.com/thevarunshah) wrote an awesome backend and still maintains it! He nicely shared stats as his system was the first HackRU tech to cope with QRs.

The Gavel updates were really small and not very difficult. [Devin](https://github.com/100) finished them in 4 or 5 Git commits over the Spring break.

Another convention that was established here, accidentally, was the R&D would be responsible for registration on the day-of. This was because only we knew all the edge-cases with the phone apps and registration systems.

## The First HackRU

The eve of the first HackRU did not feel like a victory: Qasim was coding until midnight and the R&D meeting the night before had run on until 2 am with dashboard, the app, and parts of the slackbot continuously being
fixed. That night was the first for which we had the calendar too, so there was a lot of work!

Even as registration opened, R&D felt like a losing proposition: the dashboard was bugging out and hackers could barely access their QR codes.

Then, in a miraculous thirty minutes, the thirty just before hacking began, the dashboard started to work.

After this, most of R&D was smooth sailing. The mentorship bot crashed repeatedly, but one of the bugs was a certain lack of mentors. The QR codes were a revelation for the food team and the T-shirt handout at midnight,
since both ran perfectly and each hacker took very few second to process. In fact, for the first time, lines had had to be stopped so that too many hackers would not be in the food area or getting T-shirts at the same time.

The Gavel tune-up was not a tune-up: Heroku's timeout made the web scraping intractable and led to us having to fill in the database by hand. Judging was delayed by half an hour.

Overall, R&D was OK. There were improvements to be made, but that was all.
