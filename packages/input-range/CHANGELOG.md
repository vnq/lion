# Change Log

## 0.10.0

### Minor Changes

- 0ddd38c0: member descriptions for editors and api tables

### Patch Changes

- @lion/input@0.14.1

## 0.9.0

### Minor Changes

- 02e4f2cb: add simulator to demos

### Patch Changes

- Updated dependencies [02e4f2cb]
  - @lion/core@0.17.0
  - @lion/input@0.14.0
  - @lion/localize@0.19.0

## 0.8.1

### Patch Changes

- Updated dependencies [f0527583]
  - @lion/input@0.13.1

## 0.8.0

### Minor Changes

- 43e4bb81: Type fixes and enhancements:

  - all protected/private entries added to form-core type definitions, and their dependents were fixed
  - a lot @ts-expect-error and @ts-ignore (all `get slots()` and `get modelValue()` issues are fixed)
  - categorized @ts-expect-error / @ts-ignore into:
    - [external]: when a 3rd party didn't ship types (could also be browser specs)
    - [allow-protected]: when we are allowed to know about protected methods. For instance when code
      resides in the same package
    - [allow-private]: when we need to check a private value inside a test
    - [allow]: miscellaneous allows
    - [editor]: when the editor complains, but the cli/ci doesn't

### Patch Changes

- 97b8592c: Remove lion references in docs for easier extending
- 77a04245: add protected and private type info
- Updated dependencies [77a04245]
- Updated dependencies [43e4bb81]
  - @lion/core@0.16.0
  - @lion/input@0.13.0
  - @lion/localize@0.18.0

## 0.7.3

### Patch Changes

- @lion/input@0.12.3

## 0.7.2

### Patch Changes

- @lion/input@0.12.2

## 0.7.1

### Patch Changes

- @lion/input@0.12.1

## 0.7.0

### Minor Changes

- f3e54c56: Publish documentation with a format for Rocket
- 5db622e9: BREAKING: Align exports fields. This means no more wildcards, meaning you always import with bare import specifiers, extensionless. Import components where customElements.define side effect is executed by importing from '@lion/package/define'. For multi-component packages this defines all components (e.g. radio-group + radio). If you want to only import a single one, do '@lion/radio-group/define-radio' for example for just lion-radio.

### Patch Changes

- Updated dependencies [f3e54c56]
- Updated dependencies [5db622e9]
  - @lion/core@0.15.0
  - @lion/input@0.12.0
  - @lion/localize@0.17.0

## 0.6.5

### Patch Changes

- dbacafa5: Type static get properties as {any} since the real class fields are typed separately and lit properties are just "configuring". Remove expect error.
- Updated dependencies [dbacafa5]
  - @lion/input@0.11.5

## 0.6.4

### Patch Changes

- Updated dependencies [701aadce]
  - @lion/core@0.14.1
  - @lion/localize@0.16.1
  - @lion/input@0.11.4

## 0.6.3

### Patch Changes

- @lion/input@0.11.3

## 0.6.2

### Patch Changes

- @lion/input@0.11.2

## 0.6.1

### Patch Changes

- @lion/input@0.11.1

## 0.6.0

### Minor Changes

- b2f981db: Add exports field in package.json

  Note that some tools can break with this change as long as they respect the exports field. If that is the case, check that you always access the elements included in the exports field, with the same name which they are exported. Any item not exported is considered private to the package and should not be accessed from the outside.

### Patch Changes

- Updated dependencies [b2f981db]
  - @lion/core@0.14.0
  - @lion/input@0.11.0
  - @lion/localize@0.16.0

## 0.5.16

### Patch Changes

- @lion/input@0.10.16

## 0.5.15

### Patch Changes

- @lion/input@0.10.15

## 0.5.14

### Patch Changes

- Updated dependencies [8fb7e7a1]
- Updated dependencies [9112d243]
  - @lion/core@0.13.8
  - @lion/localize@0.15.5
  - @lion/input@0.10.14

## 0.5.13

### Patch Changes

- 5302ec89: Minimise dependencies by removing integration demos to form-integrations and form-core packages.
- 98f1bb7e: Ensure all lit imports are imported from @lion/core. Remove devDependencies in all subpackages and move to root package.json. Add demo dependencies as real dependencies for users that extend our docs/demos.
- Updated dependencies [a8cf4215]
- Updated dependencies [5302ec89]
- Updated dependencies [98f1bb7e]
  - @lion/localize@0.15.4
  - @lion/input@0.10.13
  - @lion/core@0.13.7

## 0.5.12

### Patch Changes

- Updated dependencies [9fba9007]
  - @lion/core@0.13.6
  - @lion/form-core@0.6.14
  - @lion/input@0.10.12
  - @lion/localize@0.15.3

## 0.5.11

### Patch Changes

- Updated dependencies [41edf033]
  - @lion/core@0.13.5
  - @lion/form-core@0.6.13
  - @lion/input@0.10.11
  - @lion/localize@0.15.2

## 0.5.10

### Patch Changes

- Updated dependencies [5553e43e]
  - @lion/form-core@0.6.12
  - @lion/input@0.10.10

## 0.5.9

### Patch Changes

- Updated dependencies [aa8ad0e6]
- Updated dependencies [4bacc17b]
  - @lion/form-core@0.6.11
  - @lion/input@0.10.9
  - @lion/localize@0.15.1

## 0.5.8

### Patch Changes

- Updated dependencies [c5c4d4ba]
- Updated dependencies [3ada1aef]
  - @lion/form-core@0.6.10
  - @lion/localize@0.15.0
  - @lion/input@0.10.8

## 0.5.7

### Patch Changes

- Updated dependencies [cf0967fe]
  - @lion/form-core@0.6.9
  - @lion/input@0.10.7

## 0.5.6

### Patch Changes

- Updated dependencies [b222fd78]
  - @lion/form-core@0.6.8
  - @lion/input@0.10.6

## 0.5.5

### Patch Changes

- cfbcccb5: Fix type imports to reuse lion where possible, in case Lit updates with new types that may break us.
- Updated dependencies [cfbcccb5]
  - @lion/core@0.13.4
  - @lion/form-core@0.6.7
  - @lion/input@0.10.5
  - @lion/localize@0.14.9

## 0.5.4

### Patch Changes

- Updated dependencies [e2e4deec]
- Updated dependencies [8ca71b8f]
  - @lion/core@0.13.3
  - @lion/localize@0.14.8
  - @lion/form-core@0.6.6
  - @lion/input@0.10.4

## 0.5.3

### Patch Changes

- Updated dependencies [20ba0ca8]
- Updated dependencies [618f2698]
  - @lion/core@0.13.2
  - @lion/localize@0.14.7
  - @lion/form-core@0.6.5
  - @lion/input@0.10.3

## 0.5.2

### Patch Changes

- Updated dependencies [7682e520]
- Updated dependencies [2907649b]
- Updated dependencies [68e3e749]
- Updated dependencies [fd297a28]
- Updated dependencies [9fcb67f0]
- Updated dependencies [247e64a3]
- Updated dependencies [e92b98a4]
  - @lion/localize@0.14.6
  - @lion/form-core@0.6.4
  - @lion/core@0.13.1
  - @lion/input@0.10.2

## 0.5.1

### Patch Changes

- Updated dependencies [d5faa459]
- Updated dependencies [0aa4480e]
  - @lion/form-core@0.6.3
  - @lion/input@0.10.1

## 0.5.0

### Minor Changes

- cfa2daf6: Added types for all other input components except for datepicker.

### Patch Changes

- Updated dependencies [4b7bea96]
- Updated dependencies [01a798e5]
- Updated dependencies [a31b7217]
- Updated dependencies [85720654]
- Updated dependencies [32202a88]
- Updated dependencies [b9327627]
- Updated dependencies [02145a06]
- Updated dependencies [32202a88]
  - @lion/form-core@0.6.2
  - @lion/core@0.13.0
  - @lion/localize@0.14.5
  - @lion/input@0.10.0

## 0.4.23

### Patch Changes

- Updated dependencies [75107a4b]
- Updated dependencies [60d5d1d3]
  - @lion/core@0.12.0
  - @lion/form-core@0.6.1
  - @lion/input@0.9.2
  - @lion/localize@0.14.4

## 0.4.22

### Patch Changes

- Updated dependencies [874ff483]
  - @lion/form-core@0.6.0
  - @lion/core@0.11.0
  - @lion/input@0.9.1
  - @lion/localize@0.14.3

## 0.4.21

### Patch Changes

- Updated dependencies [65ecd432]
- Updated dependencies [4dc621a0]
  - @lion/core@0.10.0
  - @lion/form-core@0.5.0
  - @lion/input@0.9.0
  - @lion/localize@0.14.2

## 0.4.20

### Patch Changes

- Updated dependencies [c347fce4]
  - @lion/form-core@0.4.4
  - @lion/input@0.8.6

## 0.4.19

### Patch Changes

- Updated dependencies [4b3ac525]
  - @lion/core@0.9.1
  - @lion/form-core@0.4.3
  - @lion/input@0.8.5
  - @lion/localize@0.14.1

## 0.4.18

### Patch Changes

- Updated dependencies [dd021e43]
- Updated dependencies [07c598fd]
  - @lion/form-core@0.4.2
  - @lion/input@0.8.4

## 0.4.17

### Patch Changes

- Updated dependencies [fb236975]
  - @lion/form-core@0.4.1
  - @lion/input@0.8.3

## 0.4.16

### Patch Changes

- Updated dependencies [3c61fd29]
- Updated dependencies [09d96759]
- Updated dependencies [9ecab4d5]
  - @lion/form-core@0.4.0
  - @lion/core@0.9.0
  - @lion/localize@0.14.0
  - @lion/input@0.8.2

All notable changes to this project will be documented in this file.
See [Conventional Commits](https://conventionalcommits.org) for commit guidelines.

## [0.4.15](https://github.com/ing-bank/lion/compare/@lion/input-range@0.4.14...@lion/input-range@0.4.15) (2020-07-28)

**Note:** Version bump only for package @lion/input-range

## [0.4.14](https://github.com/ing-bank/lion/compare/@lion/input-range@0.4.13...@lion/input-range@0.4.14) (2020-07-27)

**Note:** Version bump only for package @lion/input-range

## [0.4.13](https://github.com/ing-bank/lion/compare/@lion/input-range@0.4.12...@lion/input-range@0.4.13) (2020-07-16)

**Note:** Version bump only for package @lion/input-range

## [0.4.12](https://github.com/ing-bank/lion/compare/@lion/input-range@0.4.11...@lion/input-range@0.4.12) (2020-07-13)

**Note:** Version bump only for package @lion/input-range

## [0.4.11](https://github.com/ing-bank/lion/compare/@lion/input-range@0.4.10...@lion/input-range@0.4.11) (2020-07-09)

**Note:** Version bump only for package @lion/input-range

## [0.4.10](https://github.com/ing-bank/lion/compare/@lion/input-range@0.4.9...@lion/input-range@0.4.10) (2020-07-09)

**Note:** Version bump only for package @lion/input-range

## [0.4.9](https://github.com/ing-bank/lion/compare/@lion/input-range@0.4.8...@lion/input-range@0.4.9) (2020-07-09)

**Note:** Version bump only for package @lion/input-range

## [0.4.8](https://github.com/ing-bank/lion/compare/@lion/input-range@0.4.7...@lion/input-range@0.4.8) (2020-07-07)

**Note:** Version bump only for package @lion/input-range

## [0.4.7](https://github.com/ing-bank/lion/compare/@lion/input-range@0.4.6...@lion/input-range@0.4.7) (2020-07-06)

**Note:** Version bump only for package @lion/input-range

## [0.4.6](https://github.com/ing-bank/lion/compare/@lion/input-range@0.4.5...@lion/input-range@0.4.6) (2020-06-18)

**Note:** Version bump only for package @lion/input-range

## [0.4.5](https://github.com/ing-bank/lion/compare/@lion/input-range@0.4.4...@lion/input-range@0.4.5) (2020-06-10)

**Note:** Version bump only for package @lion/input-range

## [0.4.4](https://github.com/ing-bank/lion/compare/@lion/input-range@0.4.3...@lion/input-range@0.4.4) (2020-06-09)

**Note:** Version bump only for package @lion/input-range

## [0.4.3](https://github.com/ing-bank/lion/compare/@lion/input-range@0.4.2...@lion/input-range@0.4.3) (2020-06-08)

**Note:** Version bump only for package @lion/input-range

## [0.4.2](https://github.com/ing-bank/lion/compare/@lion/input-range@0.4.1...@lion/input-range@0.4.2) (2020-06-08)

**Note:** Version bump only for package @lion/input-range

## [0.4.1](https://github.com/ing-bank/lion/compare/@lion/input-range@0.4.0...@lion/input-range@0.4.1) (2020-06-03)

### Bug Fixes

- remove all stories folders from npm ([1e04d06](https://github.com/ing-bank/lion/commit/1e04d06921f9d5e1a446b6d14045154ff83771c3))

# [0.4.0](https://github.com/ing-bank/lion/compare/@lion/input-range@0.3.1...@lion/input-range@0.4.0) (2020-05-29)

### Features

- merge field/validate/choice-input/form-group into @lion/form-core ([6170374](https://github.com/ing-bank/lion/commit/6170374ee8c058cb95fff79b4953b0535219e9b4))
- use markdown javascript (mdjs) for documentation ([bcd074d](https://github.com/ing-bank/lion/commit/bcd074d1fbce8754d428538df723ba402603e2c8))

## [0.3.1](https://github.com/ing-bank/lion/compare/@lion/input-range@0.3.0...@lion/input-range@0.3.1) (2020-05-27)

**Note:** Version bump only for package @lion/input-range

# [0.3.0](https://github.com/ing-bank/lion/compare/@lion/input-range@0.2.23...@lion/input-range@0.3.0) (2020-05-18)

### Features

- use singleton manager to support nested npm installations ([e2eb0e0](https://github.com/ing-bank/lion/commit/e2eb0e0077b9efed9382701461753778f63cad48))

## [0.2.23](https://github.com/ing-bank/lion/compare/@lion/input-range@0.2.22...@lion/input-range@0.2.23) (2020-04-29)

**Note:** Version bump only for package @lion/input-range

## [0.2.22](https://github.com/ing-bank/lion/compare/@lion/input-range@0.2.21...@lion/input-range@0.2.22) (2020-04-16)

### Bug Fixes

- **input-range:** securely apply css ([ada5350](https://github.com/ing-bank/lion/commit/ada5350a213f17f995d6bdedb82f387b3571a695))

## [0.2.21](https://github.com/ing-bank/lion/compare/@lion/input-range@0.2.20...@lion/input-range@0.2.21) (2020-04-02)

**Note:** Version bump only for package @lion/input-range

## [0.2.20](https://github.com/ing-bank/lion/compare/@lion/input-range@0.2.19...@lion/input-range@0.2.20) (2020-03-25)

**Note:** Version bump only for package @lion/input-range

## [0.2.19](https://github.com/ing-bank/lion/compare/@lion/input-range@0.2.18...@lion/input-range@0.2.19) (2020-03-19)

**Note:** Version bump only for package @lion/input-range

## [0.2.18](https://github.com/ing-bank/lion/compare/@lion/input-range@0.2.17...@lion/input-range@0.2.18) (2020-03-05)

**Note:** Version bump only for package @lion/input-range

## [0.2.17](https://github.com/ing-bank/lion/compare/@lion/input-range@0.2.16...@lion/input-range@0.2.17) (2020-03-04)

**Note:** Version bump only for package @lion/input-range

## [0.2.16](https://github.com/ing-bank/lion/compare/@lion/input-range@0.2.15...@lion/input-range@0.2.16) (2020-03-02)

### Bug Fixes

- normalize subclasser apis ([ce0630f](https://github.com/ing-bank/lion/commit/ce0630f32b2206813e5cfd2c7842b2faa5141591))

## [0.2.15](https://github.com/ing-bank/lion/compare/@lion/input-range@0.2.14...@lion/input-range@0.2.15) (2020-03-01)

**Note:** Version bump only for package @lion/input-range

## [0.2.14](https://github.com/ing-bank/lion/compare/@lion/input-range@0.2.13...@lion/input-range@0.2.14) (2020-02-26)

**Note:** Version bump only for package @lion/input-range

## [0.2.13](https://github.com/ing-bank/lion/compare/@lion/input-range@0.2.12...@lion/input-range@0.2.13) (2020-02-20)

### Bug Fixes

- removed FieldCustomMixin ([f44d8aa](https://github.com/ing-bank/lion/commit/f44d8aa26ae7124d8dcb251e1f66ab9beae71050))

## [0.2.12](https://github.com/ing-bank/lion/compare/@lion/input-range@0.2.11...@lion/input-range@0.2.12) (2020-02-19)

### Bug Fixes

- reduce storybook chunck sizes for more performance ([9fc5606](https://github.com/ing-bank/lion/commit/9fc560605f5dcf6e9abcf8d58079c59f12750046))

## [0.2.11](https://github.com/ing-bank/lion/compare/@lion/input-range@0.2.10...@lion/input-range@0.2.11) (2020-02-10)

**Note:** Version bump only for package @lion/input-range

## [0.2.10](https://github.com/ing-bank/lion/compare/@lion/input-range@0.2.9...@lion/input-range@0.2.10) (2020-02-06)

**Note:** Version bump only for package @lion/input-range

## [0.2.9](https://github.com/ing-bank/lion/compare/@lion/input-range@0.2.8...@lion/input-range@0.2.9) (2020-02-06)

**Note:** Version bump only for package @lion/input-range

## [0.2.8](https://github.com/ing-bank/lion/compare/@lion/input-range@0.2.7...@lion/input-range@0.2.8) (2020-02-06)

**Note:** Version bump only for package @lion/input-range

## [0.2.7](https://github.com/ing-bank/lion/compare/@lion/input-range@0.2.6...@lion/input-range@0.2.7) (2020-02-05)

**Note:** Version bump only for package @lion/input-range

## [0.2.6](https://github.com/ing-bank/lion/compare/@lion/input-range@0.2.5...@lion/input-range@0.2.6) (2020-02-05)

**Note:** Version bump only for package @lion/input-range

## [0.2.5](https://github.com/ing-bank/lion/compare/@lion/input-range@0.2.4...@lion/input-range@0.2.5) (2020-02-03)

**Note:** Version bump only for package @lion/input-range

## [0.2.4](https://github.com/ing-bank/lion/compare/@lion/input-range@0.2.3...@lion/input-range@0.2.4) (2020-01-23)

### Bug Fixes

- update links in stories ([0c53b1d](https://github.com/ing-bank/lion/commit/0c53b1d4bb4fa51820656bacfc2aece653d03182))

## [0.2.3](https://github.com/ing-bank/lion/compare/@lion/input-range@0.2.2...@lion/input-range@0.2.3) (2020-01-23)

**Note:** Version bump only for package @lion/input-range

## [0.2.2](https://github.com/ing-bank/lion/compare/@lion/input-range@0.2.1...@lion/input-range@0.2.2) (2020-01-20)

**Note:** Version bump only for package @lion/input-range

## [0.2.1](https://github.com/ing-bank/lion/compare/@lion/input-range@0.2.0...@lion/input-range@0.2.1) (2020-01-17)

### Bug Fixes

- update storybook and use main.js ([e61e0b9](https://github.com/ing-bank/lion/commit/e61e0b938ff72cc18cc0b3aa1560f2cece0c9fe6))

# [0.2.0](https://github.com/ing-bank/lion/compare/@lion/input-range@0.1.1...@lion/input-range@0.2.0) (2020-01-13)

### Features

- improved storybook demos ([89b835a](https://github.com/ing-bank/lion/commit/89b835a79998c45a28093de01f69216c35009a40))

## [0.1.1](https://github.com/ing-bank/lion/compare/@lion/input-range@0.1.0...@lion/input-range@0.1.1) (2020-01-08)

**Note:** Version bump only for package @lion/input-range

# 0.1.0 (2019-12-16)

### Features

- **input-range:** create input-range component ([d81e5ea](https://github.com/ing-bank/lion/commit/d81e5ea5477a4f6e5160830a5d9b81a9d1abbd6b))
