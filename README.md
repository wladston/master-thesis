Master thesis presented in December 2015 at DCC/UFMG (Departamento de Ciência
da Computação da Universidade Federal de Minas Gerais) by Wladston Ferreira
Filho.

The source code used to produce this research is available at
<https://github.com/wladston/teamspector>

# Outline

## Structure

* Chapter:Introduction
* Chapter:Fundamental Concepts
    - Section:Social Network Analysis
    - Section:The iMDB Dataset
    - Section:Machine Learning
* Chapter:Related Work
    - Section:Loosely Related Work
    - Section:Closely Related Work
* Chapter:Interpreting Movie Data and Predicting Success
    - Section:Interpreting the Dataset
        (Network model, data filtering, success parameters,
        characterization, performance groups)
    - Section:Defining Features for Movies
        (movie features, social features, feature-combination,
        characterization)
    - Movie Success Prediction Model
        (evaluation methodology)
* Chapter:Analysing the Success Prediction Model
    - Section:Experiments
        (feature selection and strength, experimental setup)
    - Section:Results
* Chapter:Conclusion and Future Work
     - Section:Contributions
     - Section:Discussion
     - Section:Difficulties Tackled
     - Section:Future work
     - Section:Publications

## Overview

**[INTRO]** Regarding collaboration, forming teams that perform well is an
important problem because…. Social elements is key to the problem because….
It's easy to form the network, and research shows links between social elements
and team performance. However these are not complete because… A novel approach
is… It needs a large dataset, so the iMDB is ideal because… The analisys is
non-trivial because of_. We found our model can improve the ways we currently
understand and predict team success in this context, and our contributions are
…, the rest of the work is organized as…

**[FUNDAMENTALS]** The concepts from SNA mentioned in this work are (graph,
bipartite graph, one-mode-graph, topological metrics, clique, node
contraction). Using SNA a bipartite network can be projected into a one-mode
network. Special handling is needed when using SNA metrics in projections from
a bipartite graph. We can access social characteristics from cliques in
a social graph by aggregating metrics from clique's nodes or by getting metrics
from the clique's contracted node. IMDb describes movie production generously,
but has many amateur movies that just add noise. Its movie co-authorship data
is directly mappable to a bipartite graph between movies and agents. iMDB also
provides these extra information from movies with are known to be correlated to
movie success. The ML concepts mentioned in this work are….

**[RELATED WORK]** These works find how to better form teams, these works find how
to predict team success, both do it with a different approach. These works use
a similar approach, but they have these limitations we don't. Our results alone
aren't better than previous work but can be combined with other predictive
models to previous works to improve them.

**[MODEL]** This is our model for a social network of movie producers. This is how
we filter the dataset. This is how we define movie success. This is how we
group movies based on success, and here is the characterization of the groups.
Tis is how we define topological features from teams (based on previous studies
we use these other features for control), and here is the characterization from
such features. Here is how features interact. Here is the final ML model we
created for predicting movie success.

**[ANALYSIS]** We proof that our prediction model works because of…. We know that
our features are adequate for prediction because…. These were the experiments
we made and its setup characteristics, and these are the results. These are the
meanings for all these results.

**[CONCLUSION]** Here is a summary of what we did, and here is a summary of the new
things we found. Here is how the field is changed in result of our work. Here
is the reasons we think are behind what we found. Here are the greatest
difficulties faced, and how we managed them. Here is how we think the work
should continue. Here are the publications generated from this work.

# Citation Reference

## Not So Similar

- **SNA**
    - `newman2001structure`: #sna
        Main article on deriving social networks from bibliographic data and
        characterizing it using social analysis metrics.
    - `lutter2013there`: #movie #sociology #sns
        Studies career advancement in IMDB to show that some network metrics are
        related to better career advancements, and that woman are more lilely to
        drop out of their careers in comparison to man.
    - `wasserman2015cross`: #sns #significance
        Studied citations between movies in iMDB to estimate a significance of a
        movie production. Used the inclusion in the us library of congress national
        film registry and correct indicator of high significance, found that the
        metric is performs much better than since expert, and better than groups of
        experts.
    - `elberse2007power`: #movies #performance #prediction
        Assess the impact of famous actors in movie success.
    - `fields2011analysis`: #sna #recc
        Studied social net. of musicians, found that they organize according to
        their similarity, so social parameters can be used for recommendation.
    - `stokols2008`: #team
        Studies scientific production and finds team-based work in science is
        extremely important for scientific breakthroughs.
    - `grund2012network`: #performance #inter-team-sna
        Performed social network analysis in football teams and found that network
        characteristics in graph modeling the way players pass the ball is related
        to team winning odds.
- **Team Formation**
    - `GunnA15`: #team-formation #deterministic #optmization
        Studies how to better form on-the-fly teams on robots working on human
        rescue in disaster zones.
    - `tseng2004novel`: #team-formation #nodes-qualities #optimization
        Studies optimization techniques for forming optimum teams by combining
        elements with different habilites.
    - `wi2009team`: #team-formation #optimization #nodes-qualities
        Studies optimization of team formation is business, by picking manager and
        team members based on node specialization and keywords from team's
        objective.
    - `anagnostopoulos2012online`: #team-formation #optimization #nodes-qualities
        Technique for efficiently forming teams with a minimum skill set. They
        use the iMDB database to emulate a problem in with teams needs to be formed
        from directors and actions, where genres of movies they have previously
        acted serve as the skill.

## Similar

- **Performance**
    - `chen2010impact`: #sna #small-world #performance
        Impact of small world on patent production, n=16 countries.
    - `schilling2007interfirm`: #performance #sna
        Studied n=1106 firms and found that those with dense connections to other
        films and low closeness are more likely to be innovative.
    - `nemoto2011social`: #sna #social-capital #performance
        Finds that when editors with more social capital (as defined by social
        network analysis metrics) work on an article, it reaches higher levels of
        quality faster.
    - `LiLY2013`: #sna #social-capital #performance
        Social capital can be estimated with metrics from social networks analysis,
        and researchers with more social capital publish research that have more
        impact
    - `PapagelisMZ11`: #sns #influence #degree
        Studied Flickr, found that the more connections a node has, the more
        influential it is, regardless of node credibility.
    - `singh2011network`: #performance #sna
        Specific kinds of network ties among open source developers are correlated
        with the development of more popular open source projects.
    - `Rebehy2013`: #performance #structural-hole #sna
        Studied 17 real state agents and found that their structural network hole
        constraint has a strong negative correlation to worker performance.
    - `Burt04`: #sns #performance
        Main article about structural holes.
    - `burt2005brokerage`: #sns #performance #structural-holes #social-captal
        Studies how sns and structural holes and be used to explain competitive
        advantage and social capital.
    - `burt2009structural`: #sna #performance #structutal-holes
        Shows that competitive advantage is created from differences in access to
        structural holes.
    - `uzzi2005collaboration`: #small-world #sna #performance #team
        Studied network of Broadway musical producers and found that small world
        coefficient in the network is related to the production of better work.
- **Prediction**
    - `OghinaBTR2012`: #movie #performance #social-activity-mining
        Studied 70 movies, extracting textual and social network activity for
        predicting the rating the movie would have in iMDB.
    - `Ghiassi2015`: #movie #prediction #performance
        Pre-production movie revenue forecast using artificial neural networks.
    - `KimKHC13`: #movie #forecast #social-activity-mining
        Shows that mining a large number of comments from social network services
        can capture the public opinion related to a movie, and help forecast
        whether the movie would be a hit.
    - `COSN2013`: #sns #prediction
        Uses financial data to predict success of kickstart fund-raising campaign,
        and an extra set of features extracted from social characteristics of
        backers and social network activity on twitter. They find that doing a
        combined predictor using both features yields the best results, with the
        social features providing a relative improvement of 4%.

# Reference

On producing a good thesis
https://www.ece.nus.edu.sg/stfpage/eleamk/phd/phdth2.html
