Source: https://youtu.be/TySnDdKz-DY?si=Td0KoGkMe4uW2KUu

0:05
all right uh I'm really excited about
0:07
these next two sessions because uh they
0:08
go hand inand uh first we're going to
0:12
learn a little bit more about some of
0:13
the new capabilities in agents and how
0:16
they make it even easier to have ai
0:19
operate the applications that you've
0:21
been building and then uh add automation
0:24
uh and then we'll see what that looks
0:26
like in production to uh to kick us off
0:28
here's Natasha hi hi hello everyone you
0:31
all look wonderful I'm uh really excited
0:34
to be here today to kick off day two of
0:37
Devcon 2 um great so uh I want to start
0:42
here by uh talking about ontology driven
0:45
agents and my name is Natasha armbrust
0:47
I'm a software engineer here at paler
0:50
and I'm on the AIP agents
0:53
team so I think it's helpful to start by
0:56
just defining what an agent is it's a
0:58
buzzword in the industry to day
1:00
everything's an agent nothing's an agent
1:02
um the working definition I like to use
1:04
it's a system that can accomplish a task
1:08
for you and in this way we're defining
1:10
the agent in terms of its outcome not
1:14
the tech
1:15
involved and so if you start to think
1:17
about what would you need to accomplish
1:19
tasks if someone new joined your team
1:22
they would probably need a detailed set
1:25
of instructions they would need task
1:27
specific context maybe that's training
1:30
documentation that's emails videos
1:34
images they would need the ability to
1:37
take action send an email open a ticket
1:39
resolve a
1:41
ticket you would hopefully have some
1:43
evalu evaluation metric for that person
1:48
and ideally they would be improving over
1:50
time and ramping up to your team and
1:54
I'll argue that these are actually The
1:56
crucial pieces that llms need in order
1:59
to accomplish
2:00
tasks so to give you some of an idea of
2:03
one version of an agent there are many
2:06
different versions this is the
2:07
architecture of AIP agents and I know
2:10
the font's small here but I think the
2:12
point that I want to make is that the
2:14
llm is a very important part of the
2:17
system it's the brains of the operation
2:19
of AIP agents it's the agentic runtime
2:23
but it's just one piece of what's going
2:25
on in the system we also need retrieval
2:28
context in order to give the LM the
2:30
relevant information for the task at
2:32
hand we need to give the llm tools in
2:34
order to perform actions query R
2:37
anology we also need to give the llm the
2:40
ability to read and write to application
2:41
state to deploy it in the UI for the
2:44
right
2:45
task and finally we'll store you know a
2:48
conversation log between the llm and the
2:51
user so there's a lot of scaffolding
2:53
around actually the large language model
2:55
in order to make them useful in the
2:57
Enterprise
3:00
and so what I would like to do in this
3:01
presentation is actually demo going
3:04
through how to add agents to your the
3:07
workflows that you're building or your
3:09
own jobs because I think it's really
3:11
hard to actually think about how do you
3:13
go from more of an ad hoc analysis
3:17
co-pilot workflow to actually automating
3:20
your agents and so what we'll do is
3:22
we'll step through a framework that can
3:25
help you think about how to add agents
3:28
to your own work close we'll start with
3:31
tier one ad hoc analysis and we'll go
3:33
all the way up to tier 4 which is an
3:35
automated
3:37
agent and as I'm stepping through each
3:39
of these tiers moving up in Automation
3:42
and
3:43
complexity I'll also be announcing new
3:46
features that we've built on the AIP
3:48
agents team that let Builders you all um
3:52
add flexibility and customization to the
3:54
agents that you're building so I'm
3:56
really excited one of these features is
3:58
actually beta just here for you guys at
4:01
Devcon 2 so um I'm I'm excited to to
4:05
jump into it and so right now I'll I'll
4:07
move over to the
4:08
demo for this demo I'll cast myself in
4:11
the role of a financial analyst and I
4:14
need to pay attention to the Federal
4:16
Reserve specifically the Federal Open
4:19
Market Committee this is a committee
4:21
that meets every six weeks and they
4:23
decide on monetary
4:26
policy and the federal fund target range
4:29
so some things that I might need to do
4:32
from the results from these meetings I
4:35
might need to send a client
4:36
communication report I might need to
4:38
determine if the asset allocation of my
4:40
firm is correct uh these meetings are
4:43
very important to understand how markets
4:45
are moving and if anyone in the crowd is
4:47
a financial expert I am not so if this
4:50
is uh a simplification of of of the
4:54
process um bear with me because I think
4:56
there's some general General pieces uh
4:59
to part of this demo that we can take
5:04
away so I'll start here in the demo in
5:08
AIP threads which is a new product we
5:11
built in uh the AIP platform that lets
5:15
us do ad hoc
5:18
analysis in Threads I can easily drag
5:21
and drop documents from my desktop into
5:25
the product and what I'm doing here is
5:28
I'm including of the Federal Open Market
5:31
Committee minutes of um the meetings for
5:35
the past year and I can ask a question
5:38
of these
5:53
documents forget my quick uh typing here
5:57
I'll zoom in but basically uh I'm asking
6:01
can you give me a summary of the current
6:02
minutes and also how do the old minutes
6:04
foreshadow the current
6:07
results and this is something that maybe
6:11
the the first minutes if I wanted to get
6:13
answers from that that would take me you
6:15
know there it's around a 20 20 Page
6:18
document so that would take me you know
6:20
maybe half an hour but now that I start
6:22
to add all of the previous minutes from
6:24
the year I mean this is something that
6:25
would take me hours to do by
6:28
myself and in threads we have citations
6:31
so I can go back to the relevant context
6:35
confirm that where the llm is actually
6:38
getting this context I can dig deeper
6:40
for further analysis confirm that the LM
6:42
is not
6:45
hallucinating and in Threads the tool is
6:48
model agnostic so you can bring the
6:50
model that you want for the task at
6:54
hand and the feature that we are
6:56
releasing in Threads um is also the
6:59
ability to bring your own custom model
7:02
so if you have a fine tune model or if
7:04
you have a small language model you can
7:06
bring it into threads and as you bring
7:09
your own model and add that
7:11
customization user experience is not
7:13
degraded we support streaming so users
7:16
will get the same experience if you plug
7:17
and play your own you know brain of the
7:23
operation so here I'm selecting a
7:25
fine-tuned one and getting the same
7:28
citation the same
7:30
you know results from from a different
7:32
large language
7:34
model the other feature I want to uh
7:37
talk through in Threads is the ability
7:39
to uh go into relevant chunks mode so
7:43
one thing that you'll notice about LMS
7:47
is
7:49
they um have Contex windows and you can
7:53
exceed their context windows and so uh
7:56
in Threads here if I exceed the lm's
7:59
context window 128,000 tokens for GPT 40
8:03
uh for
8:04
example then we can move into relevant
8:06
chunks
8:08
mode let me upload those documents
8:15
again what relevant chunks mode does is
8:18
behind the scenes No ontology no
8:20
pipeline needed we
8:23
will chunk embed index those documents
8:27
for semantic search so doc size is no
8:30
longer an a limitation
8:33
to asking questions of your
8:35
documentation this takes a little bit
8:39
longer and I was not planning to show
8:42
this on stage so
8:44
hopefully these will load in a second
8:53
here
8:56
perfect so in Threads here I have have
8:59
this ad hoc analysis tool it's really
9:02
powerful I can start to get answers
9:04
quickly for my
9:06
documentation but I might want to do
9:08
more maybe I want to share this threads
9:11
configuration with my full team and I
9:15
don't want to have them to have to
9:17
upload these documents again these are
9:19
saved as as media sets in the platform
9:22
and so what I'll do actually is upgrade
9:24
this threads configuration to an AIP
9:27
agent AIP agents
9:34
are Compass resources in the platform
9:37
and so they have the permission
9:40
structure of AIP but they also have a
9:44
lot more tooling agents become really
9:46
powerful what I want to show is that
9:49
this agent has the documents that I
9:52
added and threads there and I can easily
9:54
pull it back into threads and anyone on
9:56
my team could do this as well
10:00
so instead of needing to go and have
10:02
everyone go through find the minutes
10:04
download it maybe keep a running
10:06
document folder of this you can just
10:07
have that bundled up in one place yeah
10:10
exactly uh oftentimes you probably
10:12
actually do want to create a custom UI
10:15
and we'll do that in a second here but
10:18
not always and in that case you can just
10:20
drag and drop it back into threads and
10:22
ask the same questions
10:29
so this is the tier 2 workflow just to
10:33
um recap tier one was that ad hoc
10:35
analysis and we um allowed you to bring
10:38
your own model now tier two is a task
10:41
specific agent and in this uh tier I
10:45
want to show you all of the cool things
10:46
you can now do once you have
10:50
agents so once I have an agent I can
10:52
bring in not only this document context
10:55
but ontology context and a new context
10:58
mode which I'll I'll show in a second
11:00
here we have tools you can query your
11:02
ontology you can run actions you can run
11:04
any function in the platform um we have
11:07
a robust versioning system you can
11:09
evaluate your agents which I'll show a
11:12
bit later um and you also are able to
11:15
pull that agent into other places in the
11:20
platform one thing I might want to do
11:22
here so I have these documents I don't
11:24
really want to have to change my agent
11:26
configuration every time my documents
11:28
change
11:30
I just want the agent to be able to run
11:32
with the latest updated documents and so
11:35
what I can do actually is move to
11:37
onology context and I'll take my
11:39
documents and I could put them in a
11:40
pipeline and bring them into the
11:42
autology I could have a data source
11:44
connection to my underlying source and
11:47
with the build system and the ontology
11:49
then you can now create uh your agent
11:52
and your agent doesn't have to change
11:53
when your documents change so this can
11:56
be as new minutes come up they are
11:58
automatically synced in in so you don't
11:59
need to go and do that manual work but
12:01
you can get started by just dragging in
12:02
those documents exactly
12:05
exactly and I might want to go even
12:07
further which is um I want to customize
12:11
the retrieval context that my llm has
12:13
for the specific task at hand there's a
12:16
whole industry around retrieval context
12:19
retrieval augmented generation and the
12:21
strategies involved there query
12:23
reranking query rewriting and what we
12:27
have found from feedback on AIP agents
12:29
is that people want that tremendous
12:31
amount of flexibility to bring that the
12:33
context that they need for the task at
12:35
hand so uh We've written already a
12:39
function here and I'll just pull it in
12:41
but what that's doing is actually using
12:44
the uh document chunks that I've already
12:47
brought into the ontology from these
12:48
Federal Open Market Committee minutes
12:51
and it's doing a quer rewrite but you
12:54
can you know see the code and write any
12:57
code you want and give that retrieved
12:59
prompt to your
13:01
agent we also have the support for
13:04
citations so you don't degrade user
13:06
experience when you increase
13:08
customizability of your agent so for
13:10
example
13:14
here we'll see that I get the same
13:16
citations back to the pages in the
13:18
document that I had
13:23
before it's like Plumbing work of having
13:26
to figure out all right if I do want to
13:29
you know do custom retrieval add
13:31
complexity and how I bring in the
13:33
relevant documents I don't need to also
13:35
go reimplement the entire UI on top of
13:37
that I can I can keep using some of that
13:39
exactly exactly but as you see here
13:42
we're still in some of a a chat
13:46
experience and we probably actually want
13:49
to deploy this agent in the UI that's
13:51
right for the task at hand so maybe I
13:54
have a dashboard here that I use um the
13:59
zoomed in it's hard to see the video but
14:01
that I used that to um watch the Federal
14:04
Open Market Committee press conferences
14:06
these press conferences happen after the
14:10
meeting and Jerome Powell talks about uh
14:13
the uh monetary policy that was decided
14:15
in the meeting and these are really
14:18
dense with information so maybe I have a
14:20
dashboard in Foundry already that lets
14:22
me watch these videos maybe I can create
14:24
my client communication report from this
14:27
but I actually want to start to automate
14:28
a
14:29
the Clicks in this application I want to
14:32
create an agentic
14:35
application what I'll do is show you
14:38
actually the application working um with
14:42
the agent in it we'll explore some of
14:44
the cool features and then we'll go
14:45
under the
14:46
hood so with this agentic application I
14:49
can select the video at
14:52
hand and auto send a prompt to my agent
14:55
to summarize the video that I've
14:56
selected so no typing needed
14:59
here just like in the document case
15:01
where we had citations back to the
15:04
relevant chunks in the document and
15:06
pages that were used we have the same
15:08
thing in the video case where we can
15:09
cite the time stamps that the llm is
15:11
pulling from so in this case the Federal
15:15
Reserve lowered its policy rate by a
15:16
full percentage point over the course of
15:18
three previous meetings let's check that
15:21
out previous meetings we lowered our
15:24
policy rate by a full percentage point
15:26
from its peak that recalibration
15:29
so I'm able to dig into any of the
15:31
context in the video that the llm pulled
15:34
from some of the other things I can do
15:37
here this metric is also fed by an AIP
15:42
agent that agent is specifically
15:44
prompted to look at the metrics in the
15:46
video the federal fund target range and
15:50
the unemployment
15:51
rate and one thing I can do here is I
15:54
can click on this metric in real time
15:57
confirm where the llm got the
16:00
information from the the video and so we
16:03
are able to get citations back into that
16:07
video here we see that you're at 4.1
16:11
unemployment rate look at that feeling
16:14
that but you know overall um this is a
16:18
good labor market you're you're at 4.1%
16:21
unemployment that's that's just so you
16:24
can have this interplay between multiple
16:26
agents in your
16:27
application what are other things I can
16:29
do here let's compare this press
16:32
conference to the press conference that
16:34
happened last year at the same
16:36
time so this is something that would
16:38
take me hours to do by myself watching
16:41
both of the videos and then compare and
16:42
contrasting the LM can help me do that
16:45
with one
16:47
click and just like in the case of one
16:50
video I can have citations back to both
16:53
videos in the context and look at both
16:56
of them in the same application so we're
16:58
starting get a really powerful
17:00
experience with our agent and getting it
17:03
in the right UI for the task at hand but
17:07
let's dig under the hood what are we
17:08
actually doing here that's allowing us
17:11
to create this agentic application
17:13
specifically there's some new features
17:15
we released on the AIP agents team I've
17:18
got my embedded agent here and it has
17:20
access to the application State
17:23
specifically the selected videos from
17:26
the um the video that I've selected here
17:29
whether that's the video I'm comparing
17:31
with or the active video and it also has
17:34
an output variable we've recently
17:37
released the feature of output variables
17:39
because
17:41
before in the agent the LM had to access
17:44
every single application variable and if
17:46
you wanted to update the application
17:48
State the LM also had to run an update
17:51
application State tool which is still
17:54
available if you want to use it um but
17:58
not not not always you want the llm to
18:00
have to do that that adds an efficiency
18:02
to the system to for something that like
18:05
should sometimes be done
18:07
deterministically so in this
18:09
case the configuration my agent has is
18:12
that the clicked on citation is actually
18:15
an output variable that determinedly
18:17
gets updated so um if
18:22
here I asked it to tell me about the
18:26
videos you can debug all of this in
18:28
agent Studio itself we have this debug
18:30
application State panel but it's going
18:32
to give me a citation and you'll notice
18:34
that on the side here zoom in uh a
18:38
little bit less um I have the ontology
18:40
context citation and if I click on a
18:43
specific part uh a specific chunk that
18:46
gets overridden and that's the new
18:48
updated value and you can pull that back
18:50
into your application so you can have
18:51
this really rich application experience
18:54
with this new feature that we've
18:56
released with the variable outputs
18:59
so we've gone through tier one ad hoc
19:02
analysis we've moved over to creating
19:04
tier 2 a task specific
19:07
agent we then went to putting that agent
19:10
in an application and creating an
19:11
agentic application the tier three
19:13
workflow here this works I showed you
19:16
here for Workshop but you can also pull
19:19
it into any thirdparty app osk app we
19:22
have platform a apis and osdk support um
19:27
and in there you were able to bring your
19:29
own application context and update any
19:31
application context but let's go one
19:34
more step far further let's create a
19:37
automated agent and so this press
19:41
conference happens every six weeks and
19:44
maybe I don't actually need to jump into
19:46
my application each time uh instead what
19:50
if I actually um just need to check out
19:53
the results if an anomaly happened so
19:57
instead I would like the agent to meet
19:59
me where I'm at which is you know in my
20:01
inbox and we've released the ability to
20:04
actually do this directly in the paler
20:08
platform with automate and agents so if
20:11
we'll jump back over to the demo
20:13
here you can now publish your AIP agents
20:17
as a function when you publish them as a
20:19
function you can pull them into code
20:21
repositories you can pull them into
20:23
automate into
20:26
workshop and I have an automation set
20:29
here to run and if I look at that
20:32
automation it's giving my agent function
20:35
a simple task
20:37
prompt to uh give me the summary and
20:40
some of the key metrics in the video and
20:42
that automation ran this morning and if
20:47
I uh look at this automation here I see
20:51
it gave me a summary it gave me some
20:53
some key metrics and let's say I
20:56
actually do detect an anomaly I do want
20:57
to jump back in I can click this button
21:00
continue analysis that jumps me back
21:03
into my application with the session
21:06
pre- started with that email response
21:09
and I can dive deeper for for for more
21:12
analysis here and so just as we went up
21:15
the tiers and went from ad hoc analysis
21:16
to automated agent we can also go back
21:18
down the
21:20
tiers one of the things you can now do
21:22
as well with agents published as
21:24
functions is you can pull them into
21:25
evaluation Suites so one of the pieces I
21:28
talked about in the beginning was what
21:30
do you need to actually accomplish tasks
21:32
and one of these one of these core
21:34
pieces is actually evaluations we've
21:36
talked about this a lot at Devcon um and
21:39
so it will be no surprise that you can
21:41
now evaluate your
21:44
agents I'll just show you really quickly
21:46
one of those that I've created already
21:48
for my metrics
21:50
agent sometimes
21:56
it so for my metrics agent
21:59
um I've created an evaluation Suite it's
22:01
supposed to respond with the right
22:02
metrics each time so I can start to have
22:06
you know test driven development for AI
22:09
one of the um the the feedback loops I
22:12
even got while making this demo was that
22:14
my agent Claude kept
22:17
apologizing uh when I gave it a video
22:20
and I was not quite sure why um and I
22:23
realized it was it was it was a part of
22:25
my prompt that had told it to specific
22:28
specifically around the right uh I it
22:31
used the word videos but it was getting
22:32
video chunks and it got confused so it
22:34
kept apologizing to me that's a small
22:37
version of a of a feedback loop but
22:39
that's kind of what you would expect is
22:40
you want to improve um kind of the
22:42
interaction over
22:44
time so what did we do here uh we'll
22:49
jump back to the tiers we went from tier
22:51
one ad hoc analysis all the way up to
22:53
tier four automated agent this might not
22:55
always be how you create your agents but
22:58
this is one framework for how to think
23:00
about adding agents to the workflows
23:03
You're Building