# Learning-as-Routing-SoME

v1 - Was fundamentally flawed (because of Causal masking & EOS token handling), but was a decent (if not deceptive) proof of concept.

v2 to v5 - Was the next series of "evolutions" (Didn't know it at the time, but this architecture was still cheating, just not as much). however during the track from v2 to v5 performed I perform most of the ablations, trying to figure out what was happening behind the scenes (while also trying to mid-max Loss & PPL).

v6 - was a crucial milestone, as up until now (I was under the impression that I've worked out all of the architectures "cheats", and was trying to formalize the scaling laws of this idea.) However after I bunch of analysis. I realized that the architecture as it stood was appearing like it was learning, but in reality it was just mid-maxing it own progress by getting really good at guessing PAD tokens, while remaining just as bad with the rest of the sequence. so after I fixed that the models performance all, but flatlined (it was still learning, but not nearly the way it appeared earlier).
