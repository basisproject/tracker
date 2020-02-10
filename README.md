# Basis Tracker

See the Issues tab for progress, features, bugs, etc.

## Roadmap

Although the [Basis paper](https://gitlab.com/basisproject/paper) is a living document, gives a good sense for what this project will attempt to accomplish. So let's use the high level goals from the paper as our project outline:

- Membership
  - [x] Anybody can join with a keypair
  - [x] Any user can start a private company (non-member company)
  - [x] Companies can be converted to member companies (syndicates)
- Regions
  - [ ] Support a set of regional parameter that can be changed by members of the region ([#54][i54])
  - [ ] Cost pool, shows how many costs a region has incurred in total, via public companies/projects ([#54][i54])
- Cost tracking
  - [x] Cost tracking algorithm using cost tags as a method for portioning costs ([#44][i44])
  - [x] Labor time tracking ([#14][i14])
    - [x] Per-occupation tracking ([#33][i33])
    - [x] Per-member and per-labor wage multiplier ([#53][i53])
  - [x] Resource tags allowing tracking of certain products as resources ([#31][i31])
  - [x] Product cost tracking
  - [ ] Service cost tracking ([#20][i20])
  - [ ] Amortization pools ([#12][i21])
  - [x] [Single-company cost simulation](https://gitlab.com/basisproject/product-costs)
  - [x] [Small-economy cost simulation](https://gitlab.com/basisproject/sim) ([#7][i7])
- Public market
  - [x] Ability for member companies to order from other member companies
  - [ ] Ability for non-member companies to order from other companies (product offerings) ([#57][i57])
  - [ ] Private transactions for consumers and market companies ([#4][i4])
  - [ ] Consumer orders ([#32][i32], [#4][i4])
  - [ ] API for market
    - [ ] Ability to securely act on user's behalf in blockchain ([#52][i52])
    - [ ] Supporting infrastructure
      - [ ] User database, wraps around Basis chain
      - [ ] Elasticsearch indexing for companies, products, orders
      - [ ] Storage system for product images etc
    - [ ] Payment system integration, storage of currency via "wallets"
      - [ ] KYC bullshit
  - [ ] UI for market
- Bank
  - [ ] Holds all transactional profits ([#55][i55])
  - [ ] Allows conversion of credits to local currency (but NOT the other way around) ([#55][i55])
  - [ ] Controls regional investment parameters ([#56][i56])
  - [ ] Currency tracking system for intermediate economies ([#65][i65])
- Credit system
  - [ ] Finalized labor hours are given as credits to company members ([#53][i53])
  - [ ] Global (not regional) "resource plan" which sets a resource value for each credit ([#58][i58])
- Regional asset tracker
  - [ ] Specific permissions for managing regional assets ([#59][i59])
  - [ ] Ability to add/remove assets to/from the system ([#59][i59])
  - [ ] Available assets can be marked *in-use* by any member company (and will no longer be available afterwards) ([#59][i59])
  - [ ] Asset usage can have determined end-date or be open ended ([#59][i59])
  - [ ] Asset costing ([#59][i59])
  - [ ] Asset collaboration ([#61][i61])
- Voting
  - [ ] Anonymous voting ([#60][i60])
  - [ ] Ability to give a per-region permission to a user or set of users (council) for a set term ([#60][i60])
    - [ ] Ability to recall appointees (workers' council) ([#60][i60])
    - [ ] Councils have an approval threshold, requiring some percentage of council members to sign a transaction for it to be accepted by the system ([#60][i60])
  - [ ] Ability to vote on specific regional parameters ([#60][i60])
    - [ ] Absolute voting: majority wins ([#60][i60])
    - [ ] Value range voting: allow variable inputs and take average of all votes ([#60][i60])
  - [ ] Liquid democracy ([#60][i60])
- Public companies/projects
  - [ ] Any member can propose a new public company/project ([#62][i62])
  - [ ] Budget of company/project (labor/resources) depends on regional support ([#62][i62])
    - [ ] Companies have ongoing monthly budgets ([#62][i62])
    - [ ] Projects have a fixed cost budget ([#62][i62])
    - [ ] Budgeted costs of companies/projects are attributed to the region's cost pool ([#62][i62])
    - [ ] Non-budgeted costs must be paid via providing products/services to consumers/companies ([#62][i62])
  - [ ] Public companies/projects can have board/council members appointed by public ([#62][i62])
  - [ ] Multi-region companies/projects ([#63][i63])
    - [ ] Two or more regions can coordinate to create a new project ([#63][i63])
    - [ ] Budgets and costs would be decided proportionally per-region based on member support ([#63][i63])
    - [ ] Board members would be decided per-region based on member support ([#63][i63])
  - [ ] Regional taxation (some portion of credits earned go to repay regional cost pool) ([#64][i64])

[i4]: https://gitlab.com/basisproject/tracker/issues/4
[i7]: https://gitlab.com/basisproject/tracker/issues/7
[i14]: https://gitlab.com/basisproject/tracker/issues/14
[i20]: https://gitlab.com/basisproject/tracker/issues/20
[i21]: https://gitlab.com/basisproject/tracker/issues/21
[i31]: https://gitlab.com/basisproject/tracker/issues/31
[i32]: https://gitlab.com/basisproject/tracker/issues/32
[i33]: https://gitlab.com/basisproject/tracker/issues/33
[i44]: https://gitlab.com/basisproject/tracker/issues/44
[i52]: https://gitlab.com/basisproject/tracker/issues/52
[i53]: https://gitlab.com/basisproject/tracker/issues/53
[i54]: https://gitlab.com/basisproject/tracker/issues/54
[i55]: https://gitlab.com/basisproject/tracker/issues/55
[i56]: https://gitlab.com/basisproject/tracker/issues/56
[i57]: https://gitlab.com/basisproject/tracker/issues/57
[i58]: https://gitlab.com/basisproject/tracker/issues/58
[i59]: https://gitlab.com/basisproject/tracker/issues/59
[i60]: https://gitlab.com/basisproject/tracker/issues/60
[i61]: https://gitlab.com/basisproject/tracker/issues/61
[i62]: https://gitlab.com/basisproject/tracker/issues/62
[i63]: https://gitlab.com/basisproject/tracker/issues/63
[i64]: https://gitlab.com/basisproject/tracker/issues/64
[i65]: https://gitlab.com/basisproject/tracker/issues/65

## Contributing

Hi, thanks for wanting to help out!

First, see if there are any uncompleted items on the [Roadmap](#roadmap) that have issues attached to them. If a roadmap item you find interesting has no issue associated with it, feel free to open a new issue! Because most of the roadmap items are high-level ideas, the issue should be marked with the label `type:discussion` so all the contributors have a chance to talk it through and work out the details. Once everyone is happy, the issue be tagged as `type:feature` and can be worked on.

[Here's a list of other issues we could use your help on!](https://gitlab.com/basisproject/tracker/issues?scope=all&utf8=%E2%9C%93&state=opened&milestone_title=Any&label_name[]=help-wanted)


