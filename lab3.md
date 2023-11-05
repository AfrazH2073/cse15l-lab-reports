Part 1: Bug

Failure inducing input for program:

Non-Failure inducing input:

Symptom: Output of running the tests:

The bug, before and after being fixed:

Before:



After:


Part 2: Grep Analysis

Grep -v "age"

<img width="514" alt="image" src="https://github.com/TTVTechTaro/cse15l-lab-reports/assets/46509287/808ce8ab-0906-476c-972d-fb2a7352bc7f">



```
 Background
        Birth weight is a composite of fetal growth and length
        of gestation, each of which has different contributors and
        different sequelae. Removing the contribution of
        understanding the determinants of fetal growth. Preterm
        birth is a prime predictor of neonatal complications,
        mortality, and developmental delay. [ 1 2 ] Also, birth
        weight may predict both short- and long-term adverse
        outcomes. For example, higher birth weight among term
        infants is associated with birth complications, [ 3 ] as
        well as reduced risk of cardiovascular disease and
        hypertension in later life, but an increased risk of
        obesity. [ 4 5 6 7 8 9 ]
        In 1996, Alexander et al. published birth weight curves
        using a 1991 nationwide United States reference, later
        updated using 1994-1996 data. [ 10 11 ] However, these
        authors included weights only for the 5 th, 10 th, 50 th,
        90 th, and 95 thpercentiles at each completed week of
        gestation. While such categorical divisions may serve for
        clinical or demographic use, many research studies have
        been hampered by the traditional classifications "small for
        (LGA), historically defined as those infants below the 10
        12 ] These divisions are arbitrary, and such gross
        categorizations may mask differences in risk within or
        between populations. In addition, associations of fetal
        growth with later disease appear to span the entire birth
        weight spectrum, and are not limited to infants above or
        below a particular cut-point. [ 13 ]
        Thus, precise determination of birth weight relative to
        determinants of intrauterine growth and the sequelae of
        altered growth. The purpose of our analysis was to create a
        more nearly continuous reference measure of birth weight
      
      
        Methods
        We obtained data from the National Center for Health
        Statistics 1999 and 2000 Natality Data Sets on CD-ROM. [ 14
        ] These public-use data files include information recorded
        on birth certificates from all 3,963,465 live births in
        1999 and 4,063,823 live births in 2000 that occurred in the
        United States. We limited analysis to singletons born to
        United States resident mothers at 22 to 44 completed weeks
        last menstrual period, and for which plurality, birth
        weight and baby's sex were recorded (n = 6,714,495). We
        next trimmed the data to exclude birth weights inconsistent
        published by Alexander et al. [ 10 ] We thus retained
        information on 6,690,717 babies.
        For each completed week of gestation, we divided the
        total number of births into 100 equally sized groups, each
        representing an increment of 1 percentile point. We then
        used a resistant nonlinear smoothing technique, 4325H, [ 15
        ] twice, to account for the same birth weight value
        straddling several percentiles within each week of
        gestation, which might represent a bias towards reporting
        round numbers of birth weight values. This approach differs
        from that used by Alexander, et al., [ 10 ] who smoothed
        in each group, except in the heaviest group. We present
        tables for all individuals, as well as those stratified by
        the baby's sex and birth order.
        For situations in which a normally distributed index of
        provide what we term a 
        z-value , printed in Table 1 (see
        additional file, worksheet 'Table 1-z-values'). In many
        analyses, a 'z-score' for a subject is determined by
        subtracting the mean and dividing by the standard deviation
        from a standardization population. The z-scores from the
        sample are interpreted as if they arise from a normally
        distributed population. In our analysis, however, we use
        data from the entire population of annual births in the
        United States, not just a sample, obviating the need for
        sampling strategies or normality assumptions. In fact, the
        distribution of birth weights at each completed week of
        gestation was not normal in this complete dataset
        (Kolmogorov-Smirnov test p < 0.01 for all weeks). For
        example, for an infant born at 427 g at 24 weeks, assuming
        a normal distribution of birth weight would assign a z
        score of -1.28 (10 thpercentile), whereas using our method
        the same infant would be assigned a z value of -1.695 (5
        thpercentile), a difference of 0.4 units. Therefore, in
        comparison with the reference group, this infant is lighter
        than it would appear using a normal distribution
        assumption.
        Additional file
        
        
        Click here for file
        In contrast to this usual practice, we first calculated
        actual percentile ranks, and then assigned z-values for
        each percentile. This amounts to a non-parametric
        transformation to a normal distribution. One can manipulate
        the z-values as if they were conventional z-scores. Thus, a
        research subject in the 5 thpercentile or with a z-value of
        -1.695 is lighter than 95% and heavier than 4% of the
        the z-value corresponding to the middle of each percentile
        step - e.g. for the 5 thpercentile, which spans babies from
        >4% to 5%, we present the z-value corresponding to 4.5%.
        Babies with weights greater than the 99 thpercentile should
        be assigned a z-value of 2.576, corresponding to 99.5%.
        We performed all analyses using SAS version 8.2 (SAS
        Institute, Cary NC), with the exception of the smoothing
        procedure, for which we used STATA version 7 (STATA
        Corporation, College Station TX)
      
      
        Results
        from a low of 2,497 at 22 weeks to a maximum of 1,677,211
        at 39 weeks. There were 3,423,215 (51.2%) boys and
        3,267,502 (48.8%) girls. A total of 2,755,841 (41.2%)
        mothers were primiparous. There were 3,979,490 (59.5%)
        infants born to non-Hispanic white mothers, and 954,021
        (14.4%) born to non-Hispanic black mothers.
        For all births, Table 2 shows the birth weight
        delineating the top of each percentile step from 1 through
        99 percent, for each completed week of gestation (see
        additional file,worksheet 'Table 2-All'). The top row of
        the table reports the number of observations represented
        per percentile cell. For example, at 24 weeks of gestation,
        there were approximately 4200 reference births, or 42
        births per cell; at 39 weeks of gestation, there were
        16,772 per cell. In Figure 1, we show that the 10 th, 50
        th, and 90 thpercentiles from this analysis of 1999 and
        2000 births are virtually identical to those published by
        Alexander et al., based upon the combined 1994-1996 birth
        cohorts. [ 11 ] This figure displays the expected
        increasing slopes during the third trimester and a leveling
        off beyond 40 weeks previously seen in menstrually dated
        pregnancies. [ 10 16 ]
        The maximum variance in the estimated percentile cut
        point occurs at the 50 thpercentile within each gestation
        week cohort. For the 24 week cohort of all births, the
        point estimate of the 50th percentile is 652 grams, and the
        95% confidence interval for the point estimate includes
        values between 648 and 655 grams. This includes the
        presented values for the 48th through 51st percentile, and
        z-values between -0.038 and 0.013. Thus the birth weight
        z-score should be treated as a covariate measured with
        error [ 17 ] though the error is very small even in this
        worst case. For more extreme percentiles at 24 weeks the
        confidence interval is smaller; for percentiles greater
        than 84 or less than 13, the interval excludes the values
        for both neighboring percentiles. Similarly, as the number
        of births per percentile increases, the confidence interval
        at 50% gets smaller. For weeks with more than 80 births per
        percentile (>28 weeks), the confidence interval even at
        50% excludes the neighboring percentiles.
        Tables 3 and 4 contain percentile limits for boys and
        girls (see additional file, worksheets 'Table 3-Males' and
        'Table 4-Females'). As others have reported, [ 11 18 ] boys
        (Figure 2). Tables 5 and 6 provide percentile values for
        firstborn and non-firstborn infants (see additional file,
        worksheets 'Table 5-Firstborn' and 'Table 6-Nonfirstborn').
        Children born to parous mothers had higher birth weights at
        Finally, Tables 7 and 8 present birth weight percentiles
        for infants born to non-Hispanic white and black mothers
        only (see additional file, worksheets 'Table 7-Whiteonly'
        and 'Table 8-Blackonly'). From approximately 33 gestational
        weeks onwards, babies born to non-Hispanic white mothers
        are heavier than those born to black mothers (Figure 4), as
        has been seen previously. [ 11 ] Table 9summarizes the
        contents of Tables 2-8.
        Tables 2 through 8 are available for investigators to
        download electronically (see additional file).
        Investigators can then compare their data against these
        their choice. In most cases, the reference data including
        all births (Table 2) should be used, and researchers
        wishing to account for infant sex, maternal race, or parity
        can do so using statistical adjustment with their own data.
        However, if such adjustment is not possible, then Tables
        3-8 can be used.
        We provide Table 10, which includes selected data from
        Tables 1, 2, 3, and 4, as an example for the use of our
        method. The percentile assigned to an infant is the
        smallest one with a value larger than the infant's birth
        weight. Thus an infant weighing 2500 grams born at 37
        completed weeks of gestation would be assigned to the 9
        thpercentile. This percentile, which includes infants from
        >8 thto 9 thpercentile, corresponds to a z-value of
        -1.372. If the investigator preferred to use the sex
        specific tables, the same infant would be at the 7
        thpercentile with a z-value of -1.514 if a boy, and at the
        11 thpercentile with a z-value of -1.254 if a girl. In some
        cases the same birth weight straddles several percentiles
        occurrence when a large number of birth weights have
        identical recorded values. In such cases, we recommend that
        users assign the mean of the z-values crossed by the single
        birth weight.
      
      
        Discussion
        In this paper, we have used 1999 and 2000 United States
        nationwide Natality databases to generate multiple
        reference percentiles for birth weight at each completed
        week of gestation. Birth weight rose in a non-linear
        higher among boys than girls, and among non-firstborn
        infants than firstborns. Near term, infants born to
        non-Hispanic white mothers were larger than those born to
        non-Hispanic blacks. Our more detailed data correspond well
        with the limited percentiles published by Alexander et al.
        (Figure 1), which have been used as a reference standard
        within the United States. [ 10 11 ] Our data should prove
        useful to investigators working to understand both the
        determinants and the sequelae of fetal growth. The
        electronic publication of these data allows for
        dissemination and widespread use of such a detailed
        reference.
        Previous studies have been hampered by the lack of a
        continuous measure of birth weight independent of
        the use of fetal growth as an outcome. The interactions
        among fetal, maternal, and environmental factors that
        influence fetal growth remain poorly understood. Removing
        first step in understanding the roles of these factors in
        determining fetal growth. [ 20 21 ] Many researchers have
        studying predictors of birth weight by using the categories
        small- (SGA), large- (LGA), and appropriate-for-gestational
        the power to detect small associations between fetal
        exposures and birth weight, unless there is a change in the
        relationship exactly at the arbitrary cutpoint. This is a
        particular problem when the size of the association is
        small in magnitude. Additionally, comparing SGA or LGA with
        AGA infants inhibits study of variation within the majority
        of babies that are AGA.
        Others have used various methods to control for
        growth. One procedure has been to use a "birth weight
        ratio." This measure is calculated by dividing an infant's
        birth weight by a reference median birth weight at the
        median is chosen, this ratio will assume a linear
        relationship between birth weight and its influences across
        the range of birth weights, which may not be correct.
        a multiple regression equation along with other potential
        predictors of birth weight. This strategy has been used to
        generate a predicted weight, against which an individual
        baby's weight can be compared. [ 16 26 ] Like the birth
        weight ratio, regression analysis also typically assumes a
        linear relationship between birth weight and gestational
        any case is not required by our method, which is based on
        actual data.
        In addition to examining determinants of fetal growth,
        to understand the influence of fetal growth on later
        outcomes. While birth weight alone may predict risk for
        adult diseases, [ 8 27 ] most published data emanate from
        an era when few premature babies survived until adulthood.
        Future studies of the early life origins of adult disease
        will require disentangling the effects of length of
        gestation from fetal growth. A continuous measure is needed
        since many studies in this field suggest associations that
        span the entire range of birth weight, and are not limited
        to birth weight extremes.
        For use of fetal growth as a predictor variable,
        previously published methods either assume a normal
        distribution of birth weights at each completed week of
        gestation, [ 20 ] or include both birth weight and
        30 ] However, these approaches are limited because they
        assume either no relationship or a linear relationship
        Our method provides comprehensive reference values from
        broadly based nationwide data without making parametric,
        functional, or other modeling assumptions. It is useful
        whether fetal growth is used as an outcome or as an
        exposure (predictor). These results are not intended to
        assign a percentile to an individual infant for clinical
        use. Rather, this approach should help researchers
        investigate the factors associated with infants born at,
        for example, the 20 thas compared with the 40 th, 60 th, or
        80 thpercentile, as well as the sequelae of such
        differences in fetal growth.
        We have trimmed the dataset prior to analysis following
        the methods of Alexander et al. [ 10 ] This procedure
        primarily excludes infants with implausibly high birth
        inaccurate dating. Investigators might therefore wish to
        consider whether study subjects well beyond the 99.5
        inclusion in any analyses. Additionally, some infants with
        despite trimming, which would tend to inflate values for
        percentiles above the median.
        Several limitations should be considered. One is that
        relatively low numbers of births at the earlier gestational
        stable. However, our major percentiles are quite consistent
        with the combined 1994-1996 data even at the earliest
        account for altitude, although few infants in the US are
        born at high altitude. In addition, infants born before
        term may have different growth patterns from those
        remaining in utero. These curves thus represent
        cross-sectional weights at birth rather than longitudinal
        fetal growth.
        last menstrual period. Some studies suggest that prenatal
        ultrasound may provide more accurate dates, even when the
        last menstrual period is recalled with apparent certainty.
        [ 31 32 ] Thus, some investigators advocate use of
        ultrasound to generate birth weight norms. [ 25 ]
        Nevertheless, the use of ultrasound reference data has
        several problems. Because prenatal ultrasounds are not
        universally performed, these reference datasets are
        generally regional. [ 26 33 ] Additionally, data are
        available only for the subset of women who receive early
        ultrasounds, and may not include women seeking prenatal
        care late in pregnancy, or those who choose not to have an
        ultrasound. Further, different institutions may use
        of a given size. Thus, the United States Natality data
        remain most representative of pregnancies throughout the
        United States, and appropriate for use as reference.
        In addition to calculating reference percentiles for all
        newborns, we have presented percentiles stratified by
        infant sex, birth order, and maternal race. Other
        researchers have advocated further adjusting estimates for
        factors such as maternal height and weight, [ 16 26 ] and
        even for weights of prior infants born to the same mother.
        [ 19 ] We fear that an overly stratified reference may
        obscure important predictors of birth weight. While sex and
        birth order are immutable, the other factors likely serve
        as surrogates for a combination of maternal exposures such
        as stress, socioeconomic position, and nutrition, and thus
        are not permanently bound to differences in fetal growth
        for future populations.
        In conclusion, we have presented a United States
        national reference standard for size at birth over a broad
        range of birth weight percentiles from 22 through 44
        completed weeks of gestation. Advances in computer
        technology now permit manipulation of such large data sets
        as well as electronic publication of multiple reference
        percentiles for widespread use. These data should prove
        useful for researchers investigating the determinants and
        sequelae of altered fetal growth.
      
      
        Competing Interests
        None declared.
      
      
        Authors' Contributions
        EO participated in the study design, analysis of data,
        and was the primary author of the manuscript. KK
        participated in the study design, analysis of data, and
        revision of the manuscript. JRE participated in the study
        design and revision of the manuscript. MWG participated in
        the study design, analysis of data, and revision of the
        manuscript. All authors read and approved the final
        manuscript.

```
grep -v "infant"

<img width="524" alt="image" src="https://github.com/TTVTechTaro/cse15l-lab-reports/assets/46509287/86fa4f59-edb5-41d6-8134-ee002f92b137">



```
        Background
        Birth weight is a composite of fetal growth and length
        of gestation, each of which has different contributors and
        different sequelae. Removing the contribution of
        gestational age to birth weight is a first step in
        understanding the determinants of fetal growth. Preterm
        birth is a prime predictor of neonatal complications,
        mortality, and developmental delay. [ 1 2 ] Also, birth
        weight may predict both short- and long-term adverse
        outcomes. For example, higher birth weight among term
        well as reduced risk of cardiovascular disease and
        hypertension in later life, but an increased risk of
        obesity. [ 4 5 6 7 8 9 ]
        In 1996, Alexander et al. published birth weight curves
        using a 1991 nationwide United States reference, later
        updated using 1994-1996 data. [ 10 11 ] However, these
        authors included weights only for the 5 th, 10 th, 50 th,
        90 th, and 95 thpercentiles at each completed week of
        gestation. While such categorical divisions may serve for
        clinical or demographic use, many research studies have
        been hampered by the traditional classifications "small for
        gestational age" (SGA) and "large for gestational age"
        thor above the 90 thpercentile at each gestational age. [
        12 ] These divisions are arbitrary, and such gross
        categorizations may mask differences in risk within or
        between populations. In addition, associations of fetal
        growth with later disease appear to span the entire birth
        below a particular cut-point. [ 13 ]
        Thus, precise determination of birth weight relative to
        gestational age is needed to understand both the
        determinants of intrauterine growth and the sequelae of
        altered growth. The purpose of our analysis was to create a
        more nearly continuous reference measure of birth weight
        for gestational age using a recent nationwide dataset.
      
      
        Methods
        We obtained data from the National Center for Health
        Statistics 1999 and 2000 Natality Data Sets on CD-ROM. [ 14
        ] These public-use data files include information recorded
        on birth certificates from all 3,963,465 live births in
        1999 and 4,063,823 live births in 2000 that occurred in the
        United States. We limited analysis to singletons born to
        United States resident mothers at 22 to 44 completed weeks
        gestational age (n = 7,609,221). We included only births in
        which the gestational age was determined from a recorded
        last menstrual period, and for which plurality, birth
        weight and baby's sex were recorded (n = 6,714,495). We
        next trimmed the data to exclude birth weights inconsistent
        with the gestational age, according to the criteria
        published by Alexander et al. [ 10 ] We thus retained
        information on 6,690,717 babies.
        For each completed week of gestation, we divided the
        total number of births into 100 equally sized groups, each
        representing an increment of 1 percentile point. We then
        used a resistant nonlinear smoothing technique, 4325H, [ 15
        ] twice, to account for the same birth weight value
        straddling several percentiles within each week of
        gestation, which might represent a bias towards reporting
        round numbers of birth weight values. This approach differs
        from that used by Alexander, et al., [ 10 ] who smoothed
        across gestational age groups. We report the highest weight
        in each group, except in the heaviest group. We present
        tables for all individuals, as well as those stratified by
        the baby's sex and birth order.
        For situations in which a normally distributed index of
        birth weight for gestational age may be desirable, we
        provide what we term a 
        z-value , printed in Table 1 (see
        additional file, worksheet 'Table 1-z-values'). In many
        analyses, a 'z-score' for a subject is determined by
        subtracting the mean and dividing by the standard deviation
        from a standardization population. The z-scores from the
        sample are interpreted as if they arise from a normally
        distributed population. In our analysis, however, we use
        data from the entire population of annual births in the
        United States, not just a sample, obviating the need for
        sampling strategies or normality assumptions. In fact, the
        distribution of birth weights at each completed week of
        gestation was not normal in this complete dataset
        (Kolmogorov-Smirnov test p < 0.01 for all weeks). For
        a normal distribution of birth weight would assign a z
        score of -1.28 (10 thpercentile), whereas using our method
        thpercentile), a difference of 0.4 units. Therefore, in
        than it would appear using a normal distribution
        assumption.
        Additional file
        
        
        Click here for file
        In contrast to this usual practice, we first calculated
        actual percentile ranks, and then assigned z-values for
        each percentile. This amounts to a non-parametric
        transformation to a normal distribution. One can manipulate
        the z-values as if they were conventional z-scores. Thus, a
        research subject in the 5 thpercentile or with a z-value of
        -1.695 is lighter than 95% and heavier than 4% of the
        reference population at that gestational age. We provide
        the z-value corresponding to the middle of each percentile
        step - e.g. for the 5 thpercentile, which spans babies from
        >4% to 5%, we present the z-value corresponding to 4.5%.
        Babies with weights greater than the 99 thpercentile should
        be assigned a z-value of 2.576, corresponding to 99.5%.
        We performed all analyses using SAS version 8.2 (SAS
        Institute, Cary NC), with the exception of the smoothing
        procedure, for which we used STATA version 7 (STATA
        Corporation, College Station TX)
      
      
        Results
        from a low of 2,497 at 22 weeks to a maximum of 1,677,211
        at 39 weeks. There were 3,423,215 (51.2%) boys and
        3,267,502 (48.8%) girls. A total of 2,755,841 (41.2%)
        mothers were primiparous. There were 3,979,490 (59.5%)
        (14.4%) born to non-Hispanic black mothers.
        For all births, Table 2 shows the birth weight
        delineating the top of each percentile step from 1 through
        99 percent, for each completed week of gestation (see
        additional file,worksheet 'Table 2-All'). The top row of
        the table reports the number of observations represented
        per percentile cell. For example, at 24 weeks of gestation,
        there were approximately 4200 reference births, or 42
        births per cell; at 39 weeks of gestation, there were
        16,772 per cell. In Figure 1, we show that the 10 th, 50
        th, and 90 thpercentiles from this analysis of 1999 and
        2000 births are virtually identical to those published by
        Alexander et al., based upon the combined 1994-1996 birth
        cohorts. [ 11 ] This figure displays the expected
        increasing slopes during the third trimester and a leveling
        off beyond 40 weeks previously seen in menstrually dated
        pregnancies. [ 10 16 ]
        The maximum variance in the estimated percentile cut
        point occurs at the 50 thpercentile within each gestation
        week cohort. For the 24 week cohort of all births, the
        point estimate of the 50th percentile is 652 grams, and the
        95% confidence interval for the point estimate includes
        values between 648 and 655 grams. This includes the
        presented values for the 48th through 51st percentile, and
        z-values between -0.038 and 0.013. Thus the birth weight
        z-score should be treated as a covariate measured with
        error [ 17 ] though the error is very small even in this
        worst case. For more extreme percentiles at 24 weeks the
        confidence interval is smaller; for percentiles greater
        than 84 or less than 13, the interval excludes the values
        for both neighboring percentiles. Similarly, as the number
        of births per percentile increases, the confidence interval
        at 50% gets smaller. For weeks with more than 80 births per
        percentile (>28 weeks), the confidence interval even at
        50% excludes the neighboring percentiles.
        Tables 3 and 4 contain percentile limits for boys and
        girls (see additional file, worksheets 'Table 3-Males' and
        'Table 4-Females'). As others have reported, [ 11 18 ] boys
        were generally heavier than girls at each gestational age
        (Figure 2). Tables 5 and 6 provide percentile values for
        worksheets 'Table 5-Firstborn' and 'Table 6-Nonfirstborn').
        Children born to parous mothers had higher birth weights at
        each gestational age, as anticipated (Figure 3). [ 18 19 ]
        Finally, Tables 7 and 8 present birth weight percentiles
        only (see additional file, worksheets 'Table 7-Whiteonly'
        and 'Table 8-Blackonly'). From approximately 33 gestational
        weeks onwards, babies born to non-Hispanic white mothers
        are heavier than those born to black mothers (Figure 4), as
        has been seen previously. [ 11 ] Table 9summarizes the
        contents of Tables 2-8.
        Tables 2 through 8 are available for investigators to
        download electronically (see additional file).
        Investigators can then compare their data against these
        reference data using the statistical software package of
        their choice. In most cases, the reference data including
        all births (Table 2) should be used, and researchers
        can do so using statistical adjustment with their own data.
        However, if such adjustment is not possible, then Tables
        3-8 can be used.
        We provide Table 10, which includes selected data from
        Tables 1, 2, 3, and 4, as an example for the use of our
        completed weeks of gestation would be assigned to the 9
        >8 thto 9 thpercentile, corresponds to a z-value of
        -1.372. If the investigator preferred to use the sex
        thpercentile with a z-value of -1.514 if a boy, and at the
        11 thpercentile with a z-value of -1.254 if a girl. In some
        cases the same birth weight straddles several percentiles
        for a given gestational age despite smoothing, particularly
        at the lowest gestational ages. This is an expected
        occurrence when a large number of birth weights have
        identical recorded values. In such cases, we recommend that
        users assign the mean of the z-values crossed by the single
        birth weight.
      
      
        Discussion
        In this paper, we have used 1999 and 2000 United States
        nationwide Natality databases to generate multiple
        reference percentiles for birth weight at each completed
        week of gestation. Birth weight rose in a non-linear
        pattern as gestational age increased. In concordance with
        published data, at each gestational age birth weights were
        higher among boys than girls, and among non-firstborn
        non-Hispanic white mothers were larger than those born to
        non-Hispanic blacks. Our more detailed data correspond well
        with the limited percentiles published by Alexander et al.
        (Figure 1), which have been used as a reference standard
        within the United States. [ 10 11 ] Our data should prove
        useful to investigators working to understand both the
        determinants and the sequelae of fetal growth. The
        electronic publication of these data allows for
        dissemination and widespread use of such a detailed
        reference.
        Previous studies have been hampered by the lack of a
        continuous measure of birth weight independent of
        gestational age. We first consider previous approaches for
        the use of fetal growth as an outcome. The interactions
        among fetal, maternal, and environmental factors that
        influence fetal growth remain poorly understood. Removing
        the contribution of gestational age to birth weight is a
        first step in understanding the roles of these factors in
        determining fetal growth. [ 20 21 ] Many researchers have
        attempted to remove the influence of gestational age when
        studying predictors of birth weight by using the categories
        small- (SGA), large- (LGA), and appropriate-for-gestational
        age (AGA). [ 22 23 ] However, this categorization reduces
        the power to detect small associations between fetal
        exposures and birth weight, unless there is a change in the
        relationship exactly at the arbitrary cutpoint. This is a
        particular problem when the size of the association is
        small in magnitude. Additionally, comparing SGA or LGA with
        of babies that are AGA.
        Others have used various methods to control for
        gestational age when investigating determinants of fetal
        growth. One procedure has been to use a "birth weight
        birth weight by a reference median birth weight at the
        given gestational age. [ 16 24 25 ] However the reference
        median is chosen, this ratio will assume a linear
        relationship between birth weight and its influences across
        the range of birth weights, which may not be correct.
        Another approach has been to include gestational age in
        a multiple regression equation along with other potential
        predictors of birth weight. This strategy has been used to
        generate a predicted weight, against which an individual
        baby's weight can be compared. [ 16 26 ] Like the birth
        weight ratio, regression analysis also typically assumes a
        linear relationship between birth weight and gestational
        age. This assumption may or may not be appropriate, but in
        any case is not required by our method, which is based on
        actual data.
        In addition to examining determinants of fetal growth,
        adjusting birth weight for gestational age is also needed
        to understand the influence of fetal growth on later
        outcomes. While birth weight alone may predict risk for
        adult diseases, [ 8 27 ] most published data emanate from
        an era when few premature babies survived until adulthood.
        Future studies of the early life origins of adult disease
        will require disentangling the effects of length of
        gestation from fetal growth. A continuous measure is needed
        since many studies in this field suggest associations that
        span the entire range of birth weight, and are not limited
        to birth weight extremes.
        For use of fetal growth as a predictor variable,
        previously published methods either assume a normal
        distribution of birth weights at each completed week of
        gestation, [ 20 ] or include both birth weight and
        gestational age in multivariable regression models. [ 28 29
        30 ] However, these approaches are limited because they
        assume either no relationship or a linear relationship
        between birth weight and gestational age.
        Our method provides comprehensive reference values from
        broadly based nationwide data without making parametric,
        functional, or other modeling assumptions. It is useful
        whether fetal growth is used as an outcome or as an
        exposure (predictor). These results are not intended to
        use. Rather, this approach should help researchers
        for example, the 20 thas compared with the 40 th, 60 th, or
        80 thpercentile, as well as the sequelae of such
        differences in fetal growth.
        We have trimmed the dataset prior to analysis following
        the methods of Alexander et al. [ 10 ] This procedure
        weights at the younger gestational ages, likely because of
        inaccurate dating. Investigators might therefore wish to
        consider whether study subjects well beyond the 99.5
        thpercentile at the youngest gestational ages have
        accurately recorded weights and gestational ages, prior to
        inaccurate gestational ages may remain in the dataset
        despite trimming, which would tend to inflate values for
        percentiles above the median.
        Several limitations should be considered. One is that
        relatively low numbers of births at the earlier gestational
        stable. However, our major percentiles are quite consistent
        with the combined 1994-1996 data even at the earliest
        gestational ages (Figure 1). [ 10 11 ] We were not able to
        term may have different growth patterns from those
        remaining in utero. These curves thus represent
        cross-sectional weights at birth rather than longitudinal
        fetal growth.
        The Natality dataset calculates gestational age from
        last menstrual period. Some studies suggest that prenatal
        ultrasound may provide more accurate dates, even when the
        last menstrual period is recalled with apparent certainty.
        [ 31 32 ] Thus, some investigators advocate use of
        ultrasound to generate birth weight norms. [ 25 ]
        Nevertheless, the use of ultrasound reference data has
        several problems. Because prenatal ultrasounds are not
        universally performed, these reference datasets are
        generally regional. [ 26 33 ] Additionally, data are
        available only for the subset of women who receive early
        ultrasounds, and may not include women seeking prenatal
        care late in pregnancy, or those who choose not to have an
        ultrasound. Further, different institutions may use
        different methods to estimate gestational age for a fetus
        of a given size. Thus, the United States Natality data
        remain most representative of pregnancies throughout the
        United States, and appropriate for use as reference.
        In addition to calculating reference percentiles for all
        newborns, we have presented percentiles stratified by
        researchers have advocated further adjusting estimates for
        factors such as maternal height and weight, [ 16 26 ] and
        [ 19 ] We fear that an overly stratified reference may
        obscure important predictors of birth weight. While sex and
        birth order are immutable, the other factors likely serve
        as surrogates for a combination of maternal exposures such
        as stress, socioeconomic position, and nutrition, and thus
        are not permanently bound to differences in fetal growth
        for future populations.
        In conclusion, we have presented a United States
        national reference standard for size at birth over a broad
        range of birth weight percentiles from 22 through 44
        completed weeks of gestation. Advances in computer
        technology now permit manipulation of such large data sets
        as well as electronic publication of multiple reference
        percentiles for widespread use. These data should prove
        useful for researchers investigating the determinants and
        sequelae of altered fetal growth.
      
      
        Competing Interests
        None declared.
      
      
        Authors' Contributions
        EO participated in the study design, analysis of data,
        and was the primary author of the manuscript. KK
        participated in the study design, analysis of data, and
        revision of the manuscript. JRE participated in the study
        design and revision of the manuscript. MWG participated in
        the study design, analysis of data, and revision of the
        manuscript. All authors read and approved the final
        manuscript.
```

Using grep -v is useful because you can filter out and exclude lines that match certain content/patterns. You can use it to invert searches, remove lines that contain certain numerical values of data, information that might be void (like removing a header and data for it that is no longer valid), removing error messages, etc. However, grep-v does not accomadate for case sensitive text, or text that does not completely match the case of the inputted expression. 

Grep - l

Grep -l "biology"

<img width="449" alt="image" src="https://github.com/TTVTechTaro/cse15l-lab-reports/assets/46509287/f1ce9b16-ac00-4996-9864-023ba165a67e">

```
1471-2105-1-1.txt
1471-2105-3-12.txt
1471-2105-3-18.txt
1471-2105-3-26.txt
1471-2105-3-30.txt
1471-2105-3-34.txt
1471-2105-3-4.txt
1471-2105-4-31.txt
1471-2121-3-4.txt
1471-2121-4-5.txt
1471-213X-1-2.txt
1471-213X-2-7.txt
1471-2148-1-1.txt
1471-2148-1-6.txt
1471-2148-2-15.txt
1471-2148-2-7.txt
1471-2148-3-4.txt
1471-2164-3-16.txt
1471-2164-3-26.txt
1471-2164-3-28.txt
1471-2164-3-32.txt
1471-2164-3-9.txt
1471-2164-4-19.txt
1471-2164-4-22.txt
1471-2164-4-23.txt
1471-2172-3-4.txt
1471-2180-2-2.txt
1471-2180-2-22.txt
1471-2180-2-38.txt
1471-2180-3-11.txt
1471-2180-3-4.txt
1471-2199-3-7.txt
1471-2202-2-16.txt
1471-2202-3-1.txt
1471-2202-3-11.txt
1471-2202-4-5.txt
1471-2261-3-4.txt
1471-2350-3-7.txt
1471-2350-4-2.txt
1471-2407-1-19.txt
1471-2407-2-11.txt
1471-2407-3-16.txt
1471-2407-3-18.txt
1471-2407-3-5.txt
1472-6750-1-11.txt
1472-6750-1-13.txt
1472-6750-2-14.txt
1472-6750-2-21.txt
1472-6750-3-11.txt
1472-6769-1-3.txt
1472-6785-1-3.txt
1472-6793-1-2.txt
1472-6807-2-3.txt
1472-6963-3-14.txt
1475-2875-1-5.txt
1475-2875-2-4.txt
1475-4924-1-10.txt
1475-925X-2-10.txt
1475-9268-1-1.txt
1476-0711-2-3.txt
1476-4598-1-8.txt
1477-7827-1-9.txt
ar118.txt
ar331.txt
ar409.txt
ar612.txt
cc1498.txt
gb-2001-2-12-research0051.txt
gb-2001-2-2-research0004.txt
gb-2001-2-4-research0012.txt
gb-2002-3-10-research0052.txt
gb-2002-3-10-research0055.txt
gb-2002-3-12-research0081.txt
gb-2002-3-12-research0082.txt
gb-2002-3-12-research0086.txt
gb-2002-3-12-research0087.txt
gb-2002-3-3-research0011.txt
gb-2002-3-7-research0037.txt
gb-2002-3-8-research0039.txt
gb-2002-3-8-research0040.txt
gb-2002-4-1-r2.txt
gb-2003-4-1-r7.txt
gb-2003-4-2-r8.txt
gb-2003-4-4-r26.txt
gb-2003-4-4-r28.txt
gb-2003-4-5-r32.txt
gb-2003-4-6-r39.txt
gb-2003-4-7-r46.txt
gb-2003-4-9-r58.txt
gb-2003-4-9-r60.txt
rr167.txt

```

grep -l "sports" 

<img width="459" alt="image" src="https://github.com/TTVTechTaro/cse15l-lab-reports/assets/46509287/3978435c-2553-4ee8-a314-8bd131b82d53">


Grep -l looks through an assortment of files, in a directory or just a collection of files, and filters out files that contain the pattern that you search for. To depict this, I did grep -l with a term that is very similar to the directory's subject since the directory is called biomed, it is more likely that the term biology appears more often in the text files that are contained. However, when I did grep-l "sports" for the same directory, only 5 files showed up, since sports is a term that wouldn't be seen as much in the files since it's not related to biomed directly, therefore grep -l only returned a few files since only a few files contained the pattern I inputted.

You can also use grep -l with multiple files that you input as part of the command, so grep -l with 3 or 4 files for example, and it will show which files out of those you inputted has an occurence of that term. In addition, you can use grep -l <expression> *.txt > variable to save the files that have that occurence in a variiable. 


grep -c

grep -c "age"

<img width="507" alt="image" src="https://github.com/TTVTechTaro/cse15l-lab-reports/assets/46509287/49a5ff70-9f32-4ff5-bcb8-9254e59e68f3">

grep -c "birth" with multiple files:

<img width="551" alt="image" src="https://github.com/TTVTechTaro/cse15l-lab-reports/assets/46509287/e0d69245-0936-4290-8338-19b6b774bf53">

Grep-c counts how many times a pattern/expression occurs in a file/files. The first example we give shows using grep-c to find occurences of the word "age" in the file we specified, and in that example "age" showed up 38 times. If we control Find on the output in a Google Doc, it should give us 38 occurences of the word "age". 

Furthermore, grep-c can also be used with multiple files in one command prompt, as specifying multiple files in the command parameters prints out the occurences of the pattern/expression inputted for each file. In our example, the word birth showed up 67 times in the 1471-2431-3-6.txt file, but it showed up zero times in the other 2 files we inputted. This can be extremely helpful for data processing and analytics, where we want to know how many times a certain variable holds true, where certain values could be, and obtain numericl, quantitative information about your files. You can also use grep -c <pattern> *txt to print out the number of occurences for all of the txt files in that directory.

grep -i 

grep-i "the"

<img width="513" alt="image" src="https://github.com/TTVTechTaro/cse15l-lab-reports/assets/46509287/cb305e38-9c52-47f8-933d-66200e2d27b2">


```
The study of gene function has been greatly advanced
        through the use of transgenic mice. Over-expression and
        ectopic expression of transgenes, as well as the expression
        of genetic variants, has facilitated the deciphering of
        complex cellular processes as well as the generation of
        the conditional deletion of 
        generating transgenic mice require the availability of well
        expression of transgenes in the lung [ 1, 2, 3, 4].
        confer expression of transgenes in the liver [ 5, 6].
        Unfortunately, the number well-characterized
        limited. This is due to the fact that, although 
        blotting techniques can rapidly characterize the expression
        patterns of genes, the identification of regulatory
        the number and genomic location of transgene integration
        both the level and site of transgene expression. These
        While this approach requires knowledge of the gene
        effect, significantly increase the repertoire of regulatory
        it ensures that a single copy of the transgene is
        introduced into a defined genomic location. The
        LacZ into specific genes during the
        approach can be successful [ 8, 9]. The downside, however,
        to express must be independently targeted to the chosen
        genomic locus. This can be tedious, especially if the rate
        of recombination at the chosen genomic locus is low. Here,
        Fig 1illustrates the overall strategy that we have used
        locus. For convenience the procedure can be considered in
        chosen based on known gene expression data. In the example
        presented here we chose the 
        expressed throughout the embryonic gut endoderm of the
        mouse and our ultimate objective is to assess the function
        14, 15]. Once the locus is chosen a targeting vector is
        resistance to G418 in mammalian cells. Importantly, the 
        loxP elements so that the promoter
        Cre-expression plasmid is transiently introduced into the 
        Cre-mediated deletion of the 
        pgk promoter results in the cells
        reverting to G418 sensitivity while retaining the 
        extremely efficient. The generation of these G418-sensitive
        Neo integrated into the 
        Hnf3 α locus form the basis for
        that will allow the introduction of transgenes to the 
        Hnf3α/Neo locus. The salient features
        allows the introduction of coding sequences into this
        processing of transgenes. Targeting of transgenes to the 
        arms of homology. The 3' arm of homology contains
        nucleotides 29 to 626 of the 
        This confirmed that deletion of the 3'-end of 
        G418 [ 16]. The 5' region of homology consisted of 4.5 kb
        into sequences encoding the untranslated 5' leader region
        Hnf3 α mRNA [ 17]. These sequences
        ensure that the site of transcriptional initiation remains
        intact after transgenes have been targeted to the 
        To ascertain whether the strategy proposed in Fig 1was
        feasible and to determine the efficiency of such an
        lacZ transgene into the 
        Hnf3 α locus. The genotype of ES cell
        clones from each step of the procedure was determined by
        Southern blot analysis of genomic DNA (Fig 3). Figs 3aand
        3bshow that the genotype of ES cells at each stage of the
        procedure could be distinguished by genomic Southern blot
        pgkloxP-Neo cassette into the 
        Hnf3 α locus following the procedure
        gancyclovir (Fig 3b). In addition to the data shown in Fig
        3b, the genotype of these colonies was confirmed by
        Southern blot using DNA fragments that corresponded to 3' 
        Neo (not shown). These correctly
        introduced into the 
        (materials and methods). The expression of Cre recombinase
        mediated recombination between the 
        loxP elements that flanked the 
        pgk promoter. Southern blot analysis
        (fig 3) shows that deletion of the 
        the 
        pgk promoter resulted in the
        the promoter is necessary for 
        Neo expression. The 
        transfected Hnf3αloxPNeo ES cells, using the approach
        which the 
        transgenes to the 
        Hnf3 α locus with the aim of
        expressing them ectopically throughout the embryonic gut
        of any open reading frame when targeted to the 
        cells. There are a number of important features associated
        post-transcriptional processing of transgenic RNA. The 5'
        arm of homology within the targeting vector defines where
        the transgene is positioned relative to the 
        Hnf3 α locus. We maintained the
        integrity of the endogenous 
        within genomic sequences encoding the untranslated leader
        of the 
        Hnf3 α mRNA (Fig 2) [ 17]. The 3' arm
        of homology consisted of the 5' end of 
        the 
        encoding the last 49 amino acids of neomycin
        phosphotransferase. Such truncation of the 
        encode resistance to G418 confirming the results of Beck 
        Therefore, ES cells that randomly integrate this targeting
        predicted that homologous recombination between the
        Neo sequences in the targeting vector
        targeting vector that contained the 
        should place expression of this transgene under the control
        collected that were resistant to G418. The genotype of the
        colonies was again ascertained by Southern blot analysis of
        genomic DNA. Fig 3α shows that introduction of the 
        LacZ transgene into the 
        recombination and contained the 
        the 
        Hnf3 α locus. These data confirm the
        We predicted that transgenes inserted into the 
        throughout the endoderm of the developing gut. To determine
        containing LacZ at the 
        were produced and all showed the same pattern of
        expressed throughout the gut, liver and at particularly
        high levels in the developing stomach. Endogenous Hnf3α is
        also expressed in the floorplate of the neural tube as well
        as the notochord. However, expression of β-galactosidase in
        undetectable in these tissues. In generating the 
        all genomic sequences lying 3' to the first intron of the 
        intron or other untranslated sequences contain regulatory
        Hnf3αLacZ in the floorplate of the
        cells, leaving the first intron intact, expression of
        β-galactosidase is readily detectable in the neural-tube
        easily targeted to a defined locus in the mouse genome in
        the chosen locus has been targeted using homologous
        efficient. Indeed in the final step, where the transgene of
        interest is targeted to the desired locus, we found that
        these ES cells by standard injection into blastocysts and
        subsequent breeding of the resulting chimeric mice. It is
        worth noting, however, that if germline transmission is the
        aim of the experiment it is important to ensure that the
        selection increases the likelihood of losing germline
        competency of the ES cells.
        The targeting of transgenes into a given locus has a
        produced by injection of DNA into the male pronucleus of
        fertilized mouse eggs. A variable number of copies of the
        transgene are then integrated into the mouse genome at
        random locations. The position and number of transgene
        copies can have a profound effect on their expression. In
        and expression of the transgene is significantly more
        predictable [ 7]. Such control over the site and level of
        unpredictable impacts on the phenotype presented by the
        Introduction of single copy transgenes into the 
        overcomes the problems associated with the integration of
        transgenes to the HPRT locus and, in addition, requires the
        the transgene. Hardouin 
        by gene trapping. Here integration of the transgene at the
        translation of the transgene was facilitated by an internal
        approach relies simply on the reconstitution of resistance
        through ectopic expression studies. This requires the
        elements that are capable of expressing transgenes in the
        the transcriptional regulatory elements have to ensure
        transgene expression during the correct developmental time
        frame. Although the expression patterns of many genes have
        limited. This is partly due to the fact that complex
        sequences that are positioned many kilobases away from the
        gene making them difficult to identify. However, the
        introduction of transgenes into specific loci allows the
        sequences, which increases the likelihood that the
        transgene will be expressed in the expected fashion.
        Using targeted ES cells also provides the potential of
        examining the effects of expressing gain-of-function or
        difficult using a conventional approach because of the need
        to establish founder mice expressing the transgene.
        established then it is possible to generate clonal embryos
        directly from these ES cells by aggregating them with
        to establish that the introduction of a 
        LacZ transgene into the 
        expression throughout the developing gut (Fig 4).
        In sum, we have described a method that facilitates the
        in the mouse genome. By selecting appropriate sequences for
        toward any specific genomic locus. We, therefore, believe
        that this approach expands the repertoire of tools
        available for genetic manipulation in the mouse and will
            as the 5' arm of homology. The 3' arm of homology was
            A Xho1/HindIII (blunt) cassette containing the Tn5 
            into an XbaI (blunt) site between the Hnf3α genomic
            sequences [ 16, 25]. The 
            deleted by the action of Cre recombinase. The 
            was also regulated by the 
            adjacent to the Hnf3α 5' arm of homology to provide
            negative selection in the presence of gancylovir.
            The transgene-targeting vector used in these
            NotI/RsrII (blunt)1.4 kb cassette containing the 5' end
            by the 
            the SphI site (blunt) of pNEB193 (New England Biolabs).
            Deletion of the 49 c-terminal codons of the 
            Neo provided the 3' arm of
            homology in the targeting vector. A 530 bp EcoRI
            fragment (blunt) containing an intron from the mouse
            was isolated from the plasmid pLacF and cloned into the
            PmeI site (blunt) of the preceding plasmid [ 26].
            Finally the 5' arm of homology was provided by a 4.5 kb
            introduced into a unique Pac1 site (blunt) in the
            from 5' genomic DNA into sequences encoding the
            lacZ into the "marked" 
            supplementing the ES cell medium with 300 μg/ml
            1/100,000 of the total electroporated cell population
            them with 4-cell stage embryos made tetraploid by
            culture were allowed to continue their development 
            in utero by transferring them to
            a pseudopregnant surrogate mother. Embryos were stained
```
grep -i "g418"

<img width="532" alt="image" src="https://github.com/TTVTechTaro/cse15l-lab-reports/assets/46509287/4c62efa8-1c47-4f31-8924-9cbb31c917de">

grep -i performs similar function as grep by itself, except that doing grep -i allows you to do a search that isn't case sensitive. While normal grep would only print out the lines that have an occurence of the pattern you inputted exactly, same lower cases and same upper cases, even if the word has different cases compared to your input variable, it will still return. In our example, even though there were occurences of capital "The" while we inputted "the" for grep -i, and inputtted "g418" for "G418", the grep -i command returned all instances of the expression despite their differing cases.

