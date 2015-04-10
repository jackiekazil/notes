# Data Science in Advertising: Or a future when we love ads

Talk link: http://us.pycon.org/2015/schedule/presentation/396/
Speaker: Soups Ranjan
Friday 12:10 p.m.–12:55 p.m.
04/10/2015


## Yelp Advertisers

National as well as local businesses
* professional services (movers, garners, plumbers, restaurants, etc)

Purchase may different ways:
* Impression package on a CPM (cost per impression) basis
* Clicks on CPC (cost per click) basis
* Leads on PPC (Pay Per Call) basis

Packages:
* CMS: $350 per month for 1,000 impressions
* CPC: Up to $350 per month w/ as many clicks as possible.

## Uniqueness of Local Adveristing

Check out [Yelp Trends](http://www.yelp.com/trends)

### Location

- Users interest in a biz reduces w/ distance
- Also vaires about category
    - Users are more sensitive to how close are restuarants
    - But less sensitive to how far is that plumber, because the plumber does the driving, not the user.

### Seasonal Effects

- Mani & Pedi in the summer
- HVAC and heater in the winter

If we could predict that there is a game day, then folks look for sports bars, then we can target and sell ads to local bars.

People are more interested in night life activities over the weekend and they are less interested in health activities during the weekend.

### Categories

Sometimes when you search of sushi, sometimes it might return a karoki bar. It turns out that when folks search for sushi, they also search for karoki bars.

The click through rate of karoki bar on a sushi bar is pretty high.

### Budgets

- If budget for Chinese advertiers "nearby"  is exhausted
- We may still show an add for a closely-related category, eg Vietnamese

## Advertising is a "Matching Problem"

Contraints:
* Finite Users
* Finite Ad budgets
* Don't know future traffic
(more)

### Ad Lifecycle

1. Candidate Ad Selection
    * Near you
    * Related to the category, etc.
2. Auto Bidder
3. CTR Prediction
4. 2nd Price Auction

### 2nd Price Auction

* Winner pays the runner-up's price
* Dominant Strategy: bid your true value

If there's a click, Blue Ligh pays: cents 8/0.10 = 80 cents

### Candidate Ad Selection

* All advertisers are indexed in Elastic Search in a geoquad.
* Location and cateogry filters.

### Auto Bidder
* Sushi chef just wants to optimize: Sushi, etc.
* Doesn't necessarily want to worry about ads.
* Yelp says -- you tell us how much you want to spend per much, and we will give you the most we can give you.

*Auto bidding system*
![17099940285_f82e4b4de3_k](https://cloud.githubusercontent.com/assets/166734/7092100/0fa8e0ce-df7d-11e4-9504-0b7b1459cd38.jpg)

![17099940285_f82e4b4de3_k](https://cloud.githubusercontent.com/assets/166734/7092154/6d0ab166-df7d-11e4-9a16-7c7ce5436f70.jpg)

### CTR Prediction

![16479814213_b84145ebb3_k](https://cloud.githubusercontent.com/assets/166734/7092167/8000b6b2-df7d-11e4-9ea3-cb7a05403b5b.jpg)

![16912200088_a6d9f91212_k](https://cloud.githubusercontent.com/assets/166734/7092162/7bb86fd2-df7d-11e4-95b9-b877e14c8d7e.jpg)

![16479821263_ac9f96a5ac_k](https://cloud.githubusercontent.com/assets/166734/7092166/7e385a4c-df7d-11e4-80b7-d0f0d8947b2a.jpg)

## Model Train Sklearn, Vowpal Wabbit & Spark

![16479855213_f2aefa0d61_k](https://cloud.githubusercontent.com/assets/166734/7092221/de4979ca-df7d-11e4-9dcf-431a89483f6c.jpg)

## Vowpal Wabbit + mrJob on EMR

![16913802669_fed2608db7_k](https://cloud.githubusercontent.com/assets/166734/7092219/dcf2e12e-df7d-11e4-88ee-43baf0a17919.jpg)

(There is so much more to this talk, but I needed to step away. This talk should really be watched via video.)
