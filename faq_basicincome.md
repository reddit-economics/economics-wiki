## FAQ: Basic Income
--------------------
(by /u/mrdannyocean, /u/integralds, and /u/besttrousers)

Basic Income, a proposal under which every person in a state gets a payment from the government, is a frequent topic of conversation.  Below are some common questions asked about Basic Income.

* **What’s the difference between a Universal Basic Income (UBI) and a Negative Income Tax (NIT)?**

UBI is a payment made to everyone.  A negative income tax specifies that for incomes below a certain amount, you are negatively taxed - that is, paid.

A simple UBI can be framed as 

* Everyone receives $X per year after taxes and pays a tax rate = t.
* *Income = (1-t)Pretax + UBI (eq1)*

A simple NIT can be framed as

* Define a cutoff income. Call it a "standard deduction" if you wish.
* If you make more than the cutoff, then you deduct the cutoff from your pretax income and pay tax rate = t on the remainder. So Income = pretax - t*(pretax-cutoff)
* If you make less than the cutoff, you pay no taxes, and in addition you get some fraction k of the difference back. Income = pretax + k*(cutoff-pretax)
* If you earn exactly the cutoff, then nothing happens. You keep your pretax income.

We can do some simple algebra to rewrite NIT income as

* above: *income = (1-t)**Pretax + t***cutoff (eq2)*
* below: *income = (1-k)**Pretax + k***cutoff (eq3)*

Those formulas look awfully similar to the UBI formula. Compare (eq1) with (eq2) and (eq3). By altering the values for 'cutoff' and 't' you can obtain whichever size UBI you want (where UBI = t***cutoff). And if t=k, then the NIT and UBI in this scenario are exactly the same.

In this treatment we used a single linear tax rate and kickback rate.  If we allow for a fully nonlinear tax schedule, then any NIT can be converted into a UBI and vice-versa. The two are mathematically identical because a nonlinear tax schedule can absorb any differences between the two policies.

* **Is a Basic Income a good idea?**

This is a [normative](https://en.wikipedia.org/wiki/Normative_statement) question rather than a [positive](https://en.wikipedia.org/wiki/Positive_statement) question.  There is no scientific way to say whether a policy like UBI is 'better' than some alternative, but we can talk about the specific features and impacts it would have.

* **How large a UBI can we afford?**

This is an enormously complicated question.  Most proposals for a UBI call for replacing most welfare-state programs with a UBI, and using the savings from eliminating those programs to fund a UBI.  The details are very tricky (assuming a United States perspective below)

* Will healthcare programs be eliminated and lumped into the UBI fund, or dealt with separately?
* How do we deal with children and education?  In theory, granting a full UBI to each child could be enough to provide a child's living expenses and education.  But there is risk that parents might spend that money imprudently and neglect their children's education.  
* Should we measure federal money only, or state/local programs as well?  
* Should we also eliminate [tax expenditures](https://en.wikipedia.org/wiki/Tax_expenditure) like mortgage-interest and healthcare deductions, which can be portrayed as middle-class welfare programs?
* How to deal with social security, which is a system you pay into and only partially redistributive?

In order to come up with a real estimate of how large a UBI the US could currently afford, choices need to be made about all these programs.  [Ed Dolan](http://www.economonitor.com/dolanecon/2014/01/13/could-we-afford-a-universal-basic-income/) has built a comprehensive estimate based around

* Healthcare programs not eliminated, considered entirely separate from UBI
* Federal programs only
* Children get a full share, with a portion held back from parent control for education
* Elimination of nearly all welfare and tax expenditures - TANF, SNAP, EITC, mortgage interest deduction, standard deduction/personal exemption, retirement saving deductions, etc.
* Current SS beneficiaries can choose between keeping SS or receiving UBI, but not both.  Future SS is gradually wound down.

Based on these parameters, the United States could afford a UBI of $4,452 per person per year based on current spending.  Any larger number would require additional revenue.

* **Will UBI reduce poverty traps?**

Yes.  Under current systems, when someone gets a job they may lose most of their welfare payments and government benefits. This means they can go from not working at all to working a full week without significantly increasing their income. This is a disincentive to work. With a UBI, those with jobs retain the same UBI payment with their salary added to it, so the disincentive to work is not as strong as before.  Greg Mankiw calls these [poverty traps](http://gregmankiw.blogspot.com/2009/11/poverty-trap.html), and a UBI would help reduce marginal tax rates on poor individuals and lessen the impact of poverty traps.

* **Will UBI reduce government bureaucracy?**

UBI might reduce bureaucracy and administrative costs, but the benefits of this are perhaps overstated.  Most goverment welfare programs have fairly low overhead.  Social Security spends less than [1% per year](https://www.ssa.gov/oact/STATS/admin.html) on administrative costs, as an example.  TANF block grants have administrative costs at [about 7%](http://www.cbpp.org/research/family-income-support/how-states-use-federal-and-state-funds-under-the-tanf-block-grant).  SNAP overhead can be measured as [low as 0.1% or as high as 5%](http://www.politifact.com/truth-o-meter/statements/2013/mar/19/michele-bachmann/michele-bachmann-says-70-percent-food-stamp-fundin/), depending on what you consider to be 'administrative costs'.

In general, federal programs have fairly low administrative costs.  UBI could probably help reduce those costs even further and produce efficiency gains by simplifying and combining programs, but those gains would be in the magnitude of a percentage point or two (since UBI would also need some overhead), and not more dramatic gains.

* **Can UBI reduce fraud/waste/abuse?**

Unlikely.  Much like administrative costs, waste and fraud are often overstated.  As an example, only [1% of SNAP funds are 'trafficked'](http://www.cbpp.org/research/snap-is-effective-and-efficient?fa=view&id=3239).  As another example, Social Security Disability Insurance has a fraud rate of [around 1%](http://thehill.com/blogs/congress-blog/economy-budget/195559-social-secuity-disability-fraud-is-rare).  While no amount of fraud is good, there is no evidence for widespread fraud in most government programs, and it's not immediately clear why a UBI program would be subject to less fraud than existing programs.


* **Will UBI lead to greater bargaining power for workers?  Will UBI lead to wide-scale voluntary unemployment?**

Like other aspects of UBI, this is also an enormously complicated question which involves many factors.

* UBI could change bargaining power by changing the [reservation wage](https://en.wikipedia.org/wiki/Reservation_wage) of workers.  Any given worker has a amount where they will not work for a wage lower than the amount.  Workers typically compare their employment situation to the alternative and a reservation wage can be found based on what happens if they were to leave their job.  If a UBI were to increase the reservation wage, leaving one's job becomes more attractive and a worker gains bargaining power.  With a higher reservation wage, more people will choose to be voluntarily unemployed.
* It's not clear-cut that UBI does increase the reservation wage.  Most obviously, the level of UBI matters tremendously to this question. In addition, Unemployment Insurance (UI) already exists as a baseline 'reservation wage'. Other forms of assistance are available as well, which would generally not be available under a UBI, and a UBI could be higher or lower than the total of current assistance.  In addition, we have to account for the fact that under current conditions the reservation wage is compared to income, but in a UBI scenario it's compared to income plus UBI.  The comparison changes from "UI vs income" to "UBI vs (UBI + income)", which alters the incentive ratios workers face.  We also have to grapple with how steep the decreasing marginal utility of money is - how much more utility is placed on meeting bare bones needs vs supplemental income?  And how should we account for the variability of access and non-permanence of current government programs?  There's not a clear answer to the myriad of factors here, so it's hard to say exactly what a  UBI's impact on the reservation wage will be, and what the overall effect on labor force participation will be.
* A UBI may decrease bargaining power and increase employment in some segments of the population, if more low-end workers seek employment.  As detailed in the poverty trap section above, UBI can actually increase the incentive to work for segments of the population caught in poverty traps with high marginal tax rates.  If these workers are primarily low-end/unskilled workers, it could lead to greater labor competition in that specific sector and decreased bargaining power.  Of course (as noted above), it's possible that the security of a UBI could raise reservation wages and increase bargaining power to offset this effect.

Overall this question involves a large number of factors, and we're unlikely to see a clear answer without actual data.  For a more technical discussion, refer to the comments section of [this post](https://www.reddit.com/r/badeconomics/comments/2twaoe/is_a_basic_income_badeconomics_no_not_really_but/).
