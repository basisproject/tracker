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
  - [ ] Labor time tracking ([#14][i14])
    - [x] Per-occupation tracking ([#33][i33])
    - [ ] Per-member and per-labor wage multiplier ([#53][i53])
  - [x] Ability for companies to order from each other
  - [x] Resource tags allowing tracking of certain products as resources ([#31][i31])
  - [x] Product cost tracking
  - [ ] Service cost tracking ([#20][i20])
  - [ ] Amortization pools ([#12][i21])
  - [x] Single-company cost simulation
  - [x] Small-economy cost simulation ([#7][i7])
- Public market
  - [ ] Private transactions for consumers and market companies ([#4][i4])
  - [ ] Consumer orders ([#32][i32], [#4][i4])
  - [ ] Product offerings (interfacing between moneyless and market economy) ([#57][i57])
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
- Credit system
  - [ ] Finalized labor hours are given as credits to company members ([#53][i53])
  - [ ] Global (not regional) "resource plan" which sets a resource value for each credit ([#58][i58])
- Regional asset tracker
  - [ ] Specific permissions for managing regional assets ([#59][i59])
  - [ ] Ability to add/remove assets to/from the system ([#59][i59])
  - [ ] Available assets can be marked *in-use* by any member company (and will no longer be available afterwards) ([#59][i59])
  - [ ] Asset usage can have determined end-date or be open ended ([#59][i59])
  - [ ] Asset costing ([#59][i59])
- Voting
  - [ ] Anonymous voting
  - [ ] Ability to give a per-region permission to a user or set of users (council) for a set term
    - [ ] Ability to recall appointees (workers' council)
    - [ ] Councils have an approval threshold, requiring some percentage of council members to sign a transaction for it to be accepted by the system
  - [ ] Ability to vote on specific regional parameters
    - [ ] Absolute voting: majority wins
    - [ ] Value range voting: allow variable inputs and take average of all votes
  - [ ] Liquid democracy
- Public companies/projects
  - [ ] Any member can propose a new public company/project
  - [ ] Budget of company/project (labor/resources) depends on regional support
    - [ ] Companies have ongoing monthly budgets
    - [ ] Projects have a fixed cost budget
    - [ ] Budgeted costs of companies/projects are attributed to the region's cost pool
    - [ ] Non-budgeted costs must be paid via providing products/services to consumers/companies
  - [ ] Public companies/projects can have board/council members appointed by public
  - [ ] Multi-region companies/projects
    - [ ] Two or more regions can coordinate to create a new project
    - [ ] Budgets and costs would be decided proportionally per-region based on member support
    - [ ] Board members would be decided per-region based on member support
  - [ ] Regional taxation (some portion of credits earned go to repay regional cost pool)

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

## Contributing

Hi, thanks for wanting to help out!

First, see if there are any uncompleted items on the [Roadmap](#roadmap) that have issues attached to them. If a roadmap item you find interesting has no issue associated with it, feel free to open a new issue! Because most of the roadmap items are high-level ideas, the issue should be marked with the label `type:discussion` so all the contributors have a chance to talk it through and work out the details. Once everyone is happy, the issue be tagged as `type:feature` and can be worked on.

[Here's a list of other issues we could use your help on!](https://gitlab.com/basisproject/tracker/issues?scope=all&utf8=%E2%9C%93&state=opened&milestone_title=Any&label_name[]=help-wanted)


