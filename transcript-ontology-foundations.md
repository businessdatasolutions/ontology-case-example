Source: https://youtu.be/dz20P3j3GMc?si=h2hOZfvhUhvizdKo

0:01
Hello, DevCon. Thank you for joining us
0:04
for our third sessions specifically
0:06
about updates to our ontology
0:08
foundations. I'm Kevin, one of the
0:10
ontology group leads at Palunteer.
0:12
I'm Laura. I'm a software engineer for
0:14
data connection and realtime voice.
0:16
We're both really excited to announce
0:18
some new foundational features coming to
0:20
the ontology specifically that will
0:22
better support and enable your agentic
0:24
workflows.
0:27
When we think about building new
0:28
features in the ontology, we reason
0:30
about them in two separate ways. One,
0:33
how do we expand the capabilities of the
0:36
platform? How do you do more with your
0:37
existing ontology? And then two, how do
0:40
we provide you with the proper guard
0:42
rails so both your users and agents can
0:44
operate in a secure and safe way? Well,
0:48
in classic Palunteer fashion, I think
0:50
the best way we can show you this is
0:51
with a demo. We're going to show you
0:53
some of our favorite recent features and
0:57
Laura thankfully built a notional
1:01
operating room scheduling app quickly
1:03
over just this weekend. I think it will
1:06
use an ontology many of you are familiar
1:07
with nurses.
1:13
Yes. So I'm going to take the role here
1:15
of a nurse. I'm in the ER. I need to
1:18
help schedule patients for operations.
1:20
But obviously for that I built an
1:23
ontology OSDK application. So I'm going
1:25
to log in as a nurse. You guys can see
1:28
here my O schedule. I have operations
1:30
that are going on across different OS.
1:32
But as a nurse I really do not have the
1:35
time to sit down in a computer and
1:37
understand the patient preference, the
1:39
blood supply, the equipment, the hours
1:42
of the nurses, the hours of the doctors.
1:44
So what if I had all those constraints
1:48
encoded in my ontology and I could
1:50
leverage the power of voice agents to
1:53
help me schedule new patient on this O.
1:55
So shall we try it out? I have a voice
1:58
agent here to help me.
2:01
Hey, I've got the board up. What do you
2:03
need?
2:04
I was wondering if you can help me
2:05
schedule Patricia Collins for a last
2:07
minute cardiac bypass.
2:10
Sure thing. Let's get Patricia Collins
2:12
on the board. How long do you expect
2:14
that cardiac bypass to run?
2:17
It should be around 3 hours.
2:21
Got it. That's 180 minutes. Running that
2:24
through the schedule. Now, let me pull
2:25
up options for that.
2:32
Looked at the whole board and cross
2:34
reference surgeon availability, patient
2:36
preferences, and room capabilities. B
2:38
fits best. Dr. Miguel Dubois in
2:41
operating room 2. three fewer moves than
2:43
the best outcome option.
2:46
So before I keep talking with my voice
2:48
agent, what just happened? My voice
2:50
agent has help me understand the
2:52
ontology constraints and come up with
2:54
three different scenarios. But those
2:57
scenarios, first of all, they're not
2:58
ephemeral. I can go around in the ER and
3:01
come back later and keep editing them.
3:03
But they're also not in production data.
3:06
I'm not editing the production data. I'm
3:08
leveraging the power of ontology
3:10
scenarios which are data persisted
3:13
sandbox that allow you to use all your
3:14
ontology toolbox your actions your
3:17
functions but without touching your live
3:20
data. So let me keep talking with my
3:23
voice agent to see if I can come up come
3:25
up with a solution that I want in
3:26
production.
3:28
Great. Can you help me figure out the
3:30
difference between option A and B? What
3:32
are the nurses hours looking like for
3:34
those?
3:36
Sure. The difference between A and B. A
3:39
gives you Dr. Aiko Patel, a top cardiac
3:41
specialist, but it takes four schedule
3:43
changes and a lot of reshuffleling. B
3:46
uses Dr. Miguel Dubois, who's not a
3:48
cardiac specialist, but has a good track
3:50
record for this procedure, and it only
3:52
needs one minor adjustment. Now, neither
3:55
option adds nurse overtime. All nurses
3:57
stay on regular hours in both scenarios.
4:01
Great. I can keep iterating with the
4:03
voice agent, but for the sake of demo,
4:05
let's say I agree with the voice agent.
4:07
I know this doctor and I'm ready to
4:09
merge it into production. I don't want
4:11
to be the one responsible in merging
4:13
into production because my role is being
4:15
on site in the ER. So, what I'm going to
4:18
do right now is I'm going to submit it
4:19
for an administrator to approve this
4:21
scenario and merge it into production.
4:24
So, let's say here I want to merge
4:26
Patricia emergency
4:29
case. So, let's submit it
4:32
and I'm going to stop my voice agent and
4:34
I'm going to quickly change hats and
4:36
take the role of an administrator. So, I
4:39
have here an incognito window where I'm
4:41
logged in as an administrator as as
4:43
admin and I'm going to log in. Oh, a new
4:46
scenario request just came in. We rename
4:49
it Patricia emergency case. So, let's
4:50
click on it. And as you can see, the
4:52
changes the nurses made have been
4:54
requested for the administrator. Again,
4:57
this is an ontology scenario. I can keep
4:59
editing. I don't need to do and merge
5:02
this into production just by the changes
5:04
that the nurses made. I can keep editing
5:06
the ontology scenario and use my toolbox
5:08
of functions and actions. Let's say I
5:10
have a little bit more context than the
5:12
nurse and I actually know that Peter
5:14
patient did not get scheduled for uh for
5:17
this morning. So I can actually keep
5:18
editing the scenario and moving it and I
5:20
can move for instance James Jones to R2.
5:23
Once I'm happy with the changes, I'm
5:25
ready to merge into production. But
5:27
before I click that button,
5:30
my job as an administrator is not just
5:33
to move things and approve the O
5:35
changes, but I also need to notify every
5:38
single one of the patients that got
5:40
scheduled to a different time. So I'm
5:43
going to leverage the power of the
5:44
ontology and voice agents once again.
5:46
Once I press that approve and merge
5:48
button, it's going to trigger an
5:50
outbound call to each one of those
5:51
patients to inform them their operation
5:54
or their appointment has been
5:55
rescheduled.
5:57
I have a phone over here. I've hooked it
5:59
up to be in this case Peter patient. So
6:01
one of the patient that's going to get
6:02
called is because I moved him is Peter
6:04
patient. Let's approve and merge and see
6:07
what happens.
6:14
So someone's calling me. I'm going to
6:16
pick it up. I don't know who this is.
6:20
Hello. This is the hospital's surgical
6:22
scheduling department calling. Could I
6:24
please confirm your full name and date
6:26
of birth to get started?
6:28
Can I get more details around the
6:29
appointment before I give you that
6:31
information?
6:35
I completely understand you're curious
6:37
about the appointment details. To
6:39
protect your privacy, I do need to
6:40
verify your identity first. Could you
6:43
share your full name and date of birth?
6:45
Yes, my full name is Peter Patient. My
6:48
date of birth is January 1st, 1999.
6:53
Thanks, Peter. Let me check that against
6:55
our records.
6:56
Welcome, Peter. Thanks for confirming
6:58
that. One second while I look into the
7:00
details of your appointment. Here are
7:02
your updated appointment details. You've
7:04
got an ACL reconstruction with Dr.
7:06
Antonio Reyes scheduled for March 4th,
7:09
2026 at 3:45 p.m. Eastern time. Does
7:12
that timing work for you? And if you
7:14
have any preferences about timing or
7:16
notes for the medical staff, feel free
7:18
to let me know. Now,
7:19
could I get more information about my
7:22
friend Patricia Collins that I think
7:24
just came into the ER?
7:28
I totally get wanting to help a friend,
7:29
but due to HIPPA, I can only share
7:31
details about your own appointment. If
7:33
Patricia needs help, she's welcome to
7:35
give us a call directly and we'd be
7:37
happy to assist her.
7:39
Great. Then, let's confirm my
7:40
appointment. But, can you let the nurse
7:42
know that I need to be scheduled in O2?
7:47
Let me make a note of that. I'll add
7:49
that to your file. All right. Your
7:51
appointment is confirmed. The
7:53
confirmation ID is cof-7B711233.
7:59
Is there anything else I can help you
8:00
with today?
8:02
No, that's all. Thank you.
8:04
Okay. So, a lot of things just happened.
8:07
I had an OSDK application that was
8:09
powered by the force of the ontology and
8:12
I use voice agents to help the nurse
8:14
initiate a new schedule.
8:16
I've also had an administrator that has
8:18
changes and approved those changes of
8:20
the of the scenario and merged into
8:22
production. Once we've merged those
8:25
changes into production to your live
8:27
data that has triggered outbound call, I
8:29
want to take a pause here and make sure
8:31
that you guys heard that it tried to
8:33
verify that I was Peter patient before
8:35
trying to give me any information as
8:37
well as like I tried to get information
8:38
about Patricia patient, but it denied
8:40
me. So keep that in mind. We'll come
8:42
back later, but I'm gonna pass it to
8:44
Kevin to explain what just happened over
8:46
here.
8:48
Cool. Can we go back to slides?
8:52
So, first of all, I just want to say it
8:54
was awesome that Laura could build all
8:55
of that in one weekend. And you might be
8:57
asking yourself, how did she do it?
9:00
Luckily, she had the entire power of the
9:02
ontology and the existing data asset
9:04
already in the platform. I want to break
9:06
down what she used step by step. First,
9:09
let's talk about how this data is
9:10
secured. Object
9:13
security policies is a new feature that
9:15
allows you to define granular policies
9:17
on your object types within the
9:20
ontology. We want to make sure
9:22
especially with the sensitive data, the
9:23
right people can only see the right
9:25
things.
9:26
So let's walk through how this works.
9:29
Consider our patient object. It's the
9:32
object with the most sensitive data, but
9:35
it's also the thing you're going to
9:36
reuse across all of your workflows. So,
9:38
let's break down how we can permission
9:40
it differently for the three users that
9:42
Laura just discussed.
9:44
First, consider the admin. Their job is
9:47
to make sure that patients know when
9:50
their their scheduled appointments are.
9:53
That doesn't mean they're providing
9:54
medical care. They don't need to see
9:55
that information. They're also not doing
9:58
anything related to insurance or any
10:00
other information. So, they also
10:01
probably don't need to see sensitive
10:02
things like your social security number.
10:05
The nurse on the other hand, they are
10:07
the ones responsible for the care and
10:11
medicine of their patients. They need to
10:14
know name, phone number. They also need
10:16
to know internal hospital information
10:18
like their risk levels. Should I be
10:20
prioritizing this patient? Do they need
10:22
someone on call all the time? Also,
10:24
their blood type and other things that
10:25
are important to day-to-day operations.
10:28
Lastly, let's consider the patient.
10:30
Patients should not see anyone else's
10:32
information, just their own. They should
10:35
be able to see their very sensitive
10:36
information because well, you got to
10:38
make sure that's right. But on the flip
10:40
side, let's say for that risk level,
10:42
that's an internal hospital detail.
10:44
They're the ones prioritizing patients
10:45
and it's not something they necessarily
10:47
want to expose to all of their patients.
10:50
This was how we secured all of the
10:52
objects that you saw within that OSDK
10:54
app within Foundry. But inherently, we
10:57
had to cross another boundary when we
10:59
made that outbound call. Making a call
11:01
to Laura's phone is an external system.
11:03
So Laura's going to talk about how the
11:04
security works there.
11:06
Perfect. So the last part you saw making
11:10
me receiving a phone call from the
11:13
hospital about Peter patient schedule.
11:15
In order to know that it needed to know
11:17
that I was Peter patient. It needed to
11:18
know my appointment details. So I kind
11:20
of want to drill down of the security
11:22
layers that we've built for those
11:23
inbound and outbound calls. The first
11:25
one is network control.
11:28
Perfect. You don't want to expose your
11:31
voice agent to the whole internet. So we
11:33
want to make sure that you have the po
11:34
power to determine the network
11:36
configuration of your voice agent. The
11:39
next one is expert controls. You don't
11:41
want to let the builder decide what data
11:43
the voice agent has. That data might be
11:46
marked. So you want to make an
11:48
information security officer of your
11:50
company be responsible for approving
11:52
that that data can get leaked over the
11:55
phone and that there enough railways on
11:57
that phone call. The next one is model
12:00
security. It's very important that some
12:02
of you have georestrictions permissions
12:04
on your model. So we want to make sure
12:06
we comply with those. So the models that
12:08
we provide you in the platform to use
12:10
follow the georestriction guarantees
12:12
that you require. And the fourth one, as
12:15
I said, it verified that I was Peter
12:18
patient before it tried to give me
12:20
information about my appointment. And
12:21
once it verified that I was Peter
12:23
patient, it did not give me information
12:24
about Patricia Collins. So, we've built
12:27
tools that you can use around your agent
12:29
to make sure your agent performs to the
12:32
standards that you want. It follows a
12:33
simple pattern to build both
12:35
deterministic and non-deterministic
12:37
workflows.
12:39
So, I'll pass it to Kevin to explain a
12:41
bit more of the security of how we did
12:43
this.
12:44
So that was just the way we secured your
12:45
data, but what about all of the other
12:47
tools we use in Foundry? Laura, can you
12:49
show us the workflow lineage?
12:51
Yes. Let's go to slides. Thank you.
12:54
Cool. First, I just want to highlight
12:56
that that ontology is as simple as I
12:58
said earlier. We had operating rooms, we
13:00
had nurses, we had surgeons, we have
13:01
patients. The thing to note is because
13:04
we used ontology native scenarios, we
13:06
were able to do all of those sandbox
13:08
changes without requiring any additional
13:10
data modeling. Let's look at the patient
13:13
object for an example of of one of those
13:16
objects.
13:18
So you can see all of those properties
13:19
as we described are here. Let's go look
13:21
at the security to see those property
13:23
those object policies in practice. You
13:27
can see we've secured every row of data
13:29
as well as those sensitive properties
13:31
and fields that are specific to the
13:33
hospital and the patient and their
13:35
communications.
13:38
Going back to the lineage, you can see
13:40
that we also had a ton of functions
13:42
pre-built in the platform. These are
13:45
your backend tools that were already
13:47
available and might be used for many
13:48
workflows. Again, in scenarios, we were
13:51
able to take advantage of those existing
13:53
functions because all of those changes
13:55
weren't just happening on the back end.
13:56
They were happening within that sandbox
13:58
within the ontology. You could call your
14:00
actions, your functions, whatever tools
14:02
you already had available.
14:04
Let's maybe take a step back from
14:06
scheduling your appointments. But let's
14:08
say I need to build even more. If
14:12
patient needed to cancel their
14:13
appointment, I need a cancellation
14:15
workflow. There are already some
14:17
functions that let me do that in this
14:19
ontology like remove nurse assignment,
14:21
remove assignment. I need to build a
14:23
single atomic function that does all of
14:25
those things when it gets cancelled. I'm
14:27
going to talk to you about how
14:29
transactions, the feature we just built,
14:31
allows us to do that.
14:35
Back to the slides.
14:39
Back to slides. Thank you. So maybe I'll
14:42
set the stage a little bit. As a
14:44
developer and as there becomes more
14:47
developers wherever you work building
14:49
different things, there's going to be
14:51
different teams owning different parts
14:53
of your business. Let's say one
14:55
developer team kn owns nurses
14:57
operations, one team owns doctor
14:58
operations, one team owns all of the
15:01
inventory.
15:02
I just want to work on appointments. I
15:05
don't want to have to think through all
15:07
the different things that it takes to
15:08
reassign a nurse, but I still want to
15:10
use their existing logic.
15:14
If I just use it without thinking too
15:16
hard, I'm going to run into a problem.
15:18
Let's say I just run a very simple piece
15:19
of logic in the front end that just
15:21
tries to run all of these. I unassign
15:23
the nurse. I un assign the room prep,
15:25
but then the call I make to unassign
15:27
doctor fails. Maybe they had a bug in
15:29
their code. Maybe there was even just a
15:31
network blip. But now I'm in a weird
15:33
state. I built an application that told
15:35
the user they were canceling their
15:38
appointment, but I still have a doctor
15:39
assigned to an appointment that doesn't
15:41
even exist.
15:42
This is why we built transactions. As an
15:45
engineer, it's incredibly important for
15:47
me to know that all of these actions
15:49
succeeded or if any of them fail, they
15:52
all fail. I either cancel the
15:54
appointment or I didn't. So in the case
15:57
that one of them fails because they're
15:59
running in a transaction, all of those
16:01
changes get none of them were ever
16:03
written into the ontology. We believe
16:05
for many of the developer here this is a
16:07
familiar but obviously powerful tool for
16:09
you to develop with
16:13
a lot.
16:15
We built some aentic workflows that were
16:17
fully leveraging the power of an
16:19
existing ontology. Specifically, they
16:21
use voice agents and live audio. And
16:23
they were able to perform what if
16:25
analysis and operations in that
16:27
persisted sandbox we call scenarios. We
16:30
provided new guardrails like object
16:31
security policies and transactions to
16:33
make sure that those agents operated in
16:36
a secure and predictable way.
16:39
Some of these features are still
16:40
actively in development, but we've made
16:42
them all available to you in some form
16:44
on your DevCon stack. Please try them
16:46
out during the hackathon and reach out
16:48
to the two of us if you have any
16:50
questions. Thanks.