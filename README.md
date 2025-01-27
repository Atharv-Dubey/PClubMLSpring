# PClubMLSpring
the beginging of the code contains an approach whcich is not part of the main submission but was used to try various models using a different logicset
Classification Approach
The code implements a novel two-stage classification strategy:

Stage 1: Particle-Level Classification
First, we classify individual particles within jets. This stage:
Treats each particle as a separate data point
Uses all four measured properties as features
Learns patterns that distinguish particles in quark jets from those in gluon jets
Produces probability estimates for each particle's origin

Stage 2: Jet-Level Classification
Then, we classify entire jets based on their particle composition. This stage:
Aggregates particle-level predictions for each jet
Creates features based on the average probabilities of containing quark/gluon particles
Makes final jet-type predictions

A Random Forest Classifier as is used to better deal with the integrations of the various properties and relations in the dataset of relations
