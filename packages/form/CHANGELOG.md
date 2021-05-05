# Change Log

## 0.11.1

### Patch Changes

- @lion/fieldset@0.19.1

## 0.11.0

### Minor Changes

- 02e4f2cb: add simulator to demos

### Patch Changes

- Updated dependencies [02e4f2cb]
  - @lion/fieldset@0.19.0

## 0.10.0

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
- Updated dependencies [97b8592c]
- Updated dependencies [77a04245]
- Updated dependencies [43e4bb81]
  - @lion/fieldset@0.18.0

## 0.9.3

### Patch Changes

- @lion/fieldset@0.17.3

## 0.9.2

### Patch Changes

- @lion/fieldset@0.17.2

## 0.9.1

### Patch Changes

- @lion/fieldset@0.17.1

## 0.9.0

### Minor Changes

- f3e54c56: Publish documentation with a format for Rocket
- 5db622e9: BREAKING: Align exports fields. This means no more wildcards, meaning you always import with bare import specifiers, extensionless. Import components where customElements.define side effect is executed by importing from '@lion/package/define'. For multi-component packages this defines all components (e.g. radio-group + radio). If you want to only import a single one, do '@lion/radio-group/define-radio' for example for just lion-radio.

### Patch Changes

- Updated dependencies [f3e54c56]
- Updated dependencies [5db622e9]
  - @lion/fieldset@0.17.0

## 0.8.5

### Patch Changes

- @lion/fieldset@0.16.5

## 0.8.4

### Patch Changes

- @lion/fieldset@0.16.4

## 0.8.3

### Patch Changes

- @lion/fieldset@0.16.3

## 0.8.2

### Patch Changes

- @lion/fieldset@0.16.2

## 0.8.1

### Patch Changes

- @lion/fieldset@0.16.1

## 0.8.0

### Minor Changes

- b2f981db: Add exports field in package.json

  Note that some tools can break with this change as long as they respect the exports field. If that is the case, check that you always access the elements included in the exports field, with the same name which they are exported. Any item not exported is considered private to the package and should not be accessed from the outside.

### Patch Changes

- Updated dependencies [b2f981db]
  - @lion/fieldset@0.16.0

## 0.7.18

### Patch Changes

- 1a5e353f: Dispatch submit event on native form node instead of calling submit() directly, which circumvents lion-form submit logic and will always do a page reload and cannot be stopped by the user.

## 0.7.17

### Patch Changes

- @lion/fieldset@0.15.16

## 0.7.16

### Patch Changes

- @lion/fieldset@0.15.15

## 0.7.15

### Patch Changes

- Updated dependencies [8fb7e7a1]
- Updated dependencies [9112d243]
  - @lion/fieldset@0.15.14

## 0.7.14

### Patch Changes

- fcc60cbf: Add example link to form demo

## 0.7.13

### Patch Changes

- 5302ec89: Minimise dependencies by removing integration demos to form-integrations and form-core packages.
- 98f1bb7e: Ensure all lit imports are imported from @lion/core. Remove devDependencies in all subpackages and move to root package.json. Add demo dependencies as real dependencies for users that extend our docs/demos.
- Updated dependencies [5302ec89]
- Updated dependencies [98f1bb7e]
  - @lion/fieldset@0.15.13

## 0.7.12

### Patch Changes

- Updated dependencies [9fba9007]
  - @lion/core@0.13.6
  - @lion/fieldset@0.15.12

## 0.7.11

### Patch Changes

- Updated dependencies [41edf033]
  - @lion/core@0.13.5
  - @lion/fieldset@0.15.11

## 0.7.10

### Patch Changes

- @lion/fieldset@0.15.10

## 0.7.9

### Patch Changes

- @lion/fieldset@0.15.9

## 0.7.8

### Patch Changes

- @lion/fieldset@0.15.8

## 0.7.7

### Patch Changes

- @lion/fieldset@0.15.7

## 0.7.6

### Patch Changes

- @lion/fieldset@0.15.6

## 0.7.5

### Patch Changes

- cfbcccb5: Fix type imports to reuse lion where possible, in case Lit updates with new types that may break us.
- Updated dependencies [cfbcccb5]
  - @lion/core@0.13.4
  - @lion/fieldset@0.15.5

## 0.7.4

### Patch Changes

- Updated dependencies [e2e4deec]
  - @lion/core@0.13.3
  - @lion/fieldset@0.15.4

## 0.7.3

### Patch Changes

- 618f2698: Run tests also on webkit
- Updated dependencies [20ba0ca8]
  - @lion/core@0.13.2
  - @lion/fieldset@0.15.3

## 0.7.2

### Patch Changes

- Updated dependencies [e92b98a4]
  - @lion/core@0.13.1
  - @lion/fieldset@0.15.2

## 0.7.1

### Patch Changes

- Updated dependencies [0aa4480e]
  - @lion/fieldset@0.15.1

## 0.7.0

### Minor Changes

- 6f08e929: Added types for form and fieldset packages.

### Patch Changes

- Updated dependencies [01a798e5]
- Updated dependencies [6f08e929]
  - @lion/core@0.13.0
  - @lion/fieldset@0.15.0

## 0.6.23

### Patch Changes

- Updated dependencies [75107a4b]
  - @lion/core@0.12.0
  - @lion/fieldset@0.14.9

## 0.6.22

### Patch Changes

- Updated dependencies [874ff483]
  - @lion/core@0.11.0
  - @lion/fieldset@0.14.8

## 0.6.21

### Patch Changes

- Updated dependencies [65ecd432]
- Updated dependencies [4dc621a0]
  - @lion/core@0.10.0
  - @lion/fieldset@0.14.7

## 0.6.20

### Patch Changes

- Updated dependencies [c347fce4]
  - @lion/fieldset@0.14.6

## 0.6.19

### Patch Changes

- Updated dependencies [4b3ac525]
  - @lion/core@0.9.1
  - @lion/fieldset@0.14.5

## 0.6.18

### Patch Changes

- dd021e43: Groups need a valid formattedValue representing the value of it's form elements
- Updated dependencies [dd021e43]
  - @lion/fieldset@0.14.4

## 0.6.17

### Patch Changes

- @lion/fieldset@0.14.3

## 0.6.16

### Patch Changes

- Updated dependencies [3c61fd29]
- Updated dependencies [9ecab4d5]
  - @lion/core@0.9.0
  - @lion/fieldset@0.14.2

All notable changes to this project will be documented in this file.
See [Conventional Commits](https://conventionalcommits.org) for commit guidelines.

## [0.6.15](https://github.com/ing-bank/lion/compare/@lion/form@0.6.14...@lion/form@0.6.15) (2020-07-28)

**Note:** Version bump only for package @lion/form

## [0.6.14](https://github.com/ing-bank/lion/compare/@lion/form@0.6.13...@lion/form@0.6.14) (2020-07-27)

**Note:** Version bump only for package @lion/form

## [0.6.13](https://github.com/ing-bank/lion/compare/@lion/form@0.6.12...@lion/form@0.6.13) (2020-07-16)

**Note:** Version bump only for package @lion/form

## [0.6.12](https://github.com/ing-bank/lion/compare/@lion/form@0.6.11...@lion/form@0.6.12) (2020-07-13)

**Note:** Version bump only for package @lion/form

## [0.6.11](https://github.com/ing-bank/lion/compare/@lion/form@0.6.10...@lion/form@0.6.11) (2020-07-09)

**Note:** Version bump only for package @lion/form

## [0.6.10](https://github.com/ing-bank/lion/compare/@lion/form@0.6.9...@lion/form@0.6.10) (2020-07-09)

**Note:** Version bump only for package @lion/form

## [0.6.9](https://github.com/ing-bank/lion/compare/@lion/form@0.6.8...@lion/form@0.6.9) (2020-07-09)

**Note:** Version bump only for package @lion/form

## [0.6.8](https://github.com/ing-bank/lion/compare/@lion/form@0.6.7...@lion/form@0.6.8) (2020-07-07)

**Note:** Version bump only for package @lion/form

## [0.6.7](https://github.com/ing-bank/lion/compare/@lion/form@0.6.6...@lion/form@0.6.7) (2020-07-06)

**Note:** Version bump only for package @lion/form

## [0.6.6](https://github.com/ing-bank/lion/compare/@lion/form@0.6.5...@lion/form@0.6.6) (2020-06-18)

**Note:** Version bump only for package @lion/form

## [0.6.5](https://github.com/ing-bank/lion/compare/@lion/form@0.6.4...@lion/form@0.6.5) (2020-06-10)

**Note:** Version bump only for package @lion/form

## [0.6.4](https://github.com/ing-bank/lion/compare/@lion/form@0.6.3...@lion/form@0.6.4) (2020-06-09)

**Note:** Version bump only for package @lion/form

## [0.6.3](https://github.com/ing-bank/lion/compare/@lion/form@0.6.2...@lion/form@0.6.3) (2020-06-08)

**Note:** Version bump only for package @lion/form

## [0.6.2](https://github.com/ing-bank/lion/compare/@lion/form@0.6.1...@lion/form@0.6.2) (2020-06-08)

**Note:** Version bump only for package @lion/form

## [0.6.1](https://github.com/ing-bank/lion/compare/@lion/form@0.6.0...@lion/form@0.6.1) (2020-06-03)

### Bug Fixes

- remove all stories folders from npm ([1e04d06](https://github.com/ing-bank/lion/commit/1e04d06921f9d5e1a446b6d14045154ff83771c3))

# [0.6.0](https://github.com/ing-bank/lion/compare/@lion/form@0.5.3...@lion/form@0.6.0) (2020-05-29)

### Features

- merge field/validate/choice-input/form-group into @lion/form-core ([6170374](https://github.com/ing-bank/lion/commit/6170374ee8c058cb95fff79b4953b0535219e9b4))
- use markdown javascript (mdjs) for documentation ([bcd074d](https://github.com/ing-bank/lion/commit/bcd074d1fbce8754d428538df723ba402603e2c8))

## [0.5.3](https://github.com/ing-bank/lion/compare/@lion/form@0.5.2...@lion/form@0.5.3) (2020-05-27)

**Note:** Version bump only for package @lion/form

## [0.5.2](https://github.com/ing-bank/lion/compare/@lion/form@0.5.1...@lion/form@0.5.2) (2020-05-27)

**Note:** Version bump only for package @lion/form

## [0.5.1](https://github.com/ing-bank/lion/compare/@lion/form@0.5.0...@lion/form@0.5.1) (2020-05-25)

**Note:** Version bump only for package @lion/form

# [0.5.0](https://github.com/ing-bank/lion/compare/@lion/form@0.4.23...@lion/form@0.5.0) (2020-05-18)

### Features

- use singleton manager to support nested npm installations ([e2eb0e0](https://github.com/ing-bank/lion/commit/e2eb0e0077b9efed9382701461753778f63cad48))

## [0.4.23](https://github.com/ing-bank/lion/compare/@lion/form@0.4.22...@lion/form@0.4.23) (2020-04-29)

**Note:** Version bump only for package @lion/form

## [0.4.22](https://github.com/ing-bank/lion/compare/@lion/form@0.4.21...@lion/form@0.4.22) (2020-04-02)

**Note:** Version bump only for package @lion/form

## [0.4.21](https://github.com/ing-bank/lion/compare/@lion/form@0.4.20...@lion/form@0.4.21) (2020-03-25)

**Note:** Version bump only for package @lion/form

## [0.4.20](https://github.com/ing-bank/lion/compare/@lion/form@0.4.19...@lion/form@0.4.20) (2020-03-19)

### Bug Fixes

- **form:** remove correct reset event listener on teardown ([9cd0ed3](https://github.com/ing-bank/lion/commit/9cd0ed364fd440353c0b4a94bb1e5001ea9415c0))

## [0.4.19](https://github.com/ing-bank/lion/compare/@lion/form@0.4.18...@lion/form@0.4.19) (2020-03-19)

**Note:** Version bump only for package @lion/form

## [0.4.18](https://github.com/ing-bank/lion/compare/@lion/form@0.4.17...@lion/form@0.4.18) (2020-03-05)

**Note:** Version bump only for package @lion/form

## [0.4.17](https://github.com/ing-bank/lion/compare/@lion/form@0.4.16...@lion/form@0.4.17) (2020-03-04)

**Note:** Version bump only for package @lion/form

## [0.4.16](https://github.com/ing-bank/lion/compare/@lion/form@0.4.15...@lion/form@0.4.16) (2020-03-02)

### Bug Fixes

- normalize subclasser apis ([ce0630f](https://github.com/ing-bank/lion/commit/ce0630f32b2206813e5cfd2c7842b2faa5141591))
- **form:** leave accessible role to native form ([1310bd4](https://github.com/ing-bank/lion/commit/1310bd491e5363ec86159c1ae390964b1fb9cc16))

## [0.4.15](https://github.com/ing-bank/lion/compare/@lion/form@0.4.14...@lion/form@0.4.15) (2020-03-01)

**Note:** Version bump only for package @lion/form

## [0.4.14](https://github.com/ing-bank/lion/compare/@lion/form@0.4.13...@lion/form@0.4.14) (2020-02-26)

**Note:** Version bump only for package @lion/form

## [0.4.13](https://github.com/ing-bank/lion/compare/@lion/form@0.4.12...@lion/form@0.4.13) (2020-02-20)

**Note:** Version bump only for package @lion/form

## [0.4.12](https://github.com/ing-bank/lion/compare/@lion/form@0.4.11...@lion/form@0.4.12) (2020-02-19)

### Bug Fixes

- reduce storybook chunck sizes for more performance ([9fc5606](https://github.com/ing-bank/lion/commit/9fc560605f5dcf6e9abcf8d58079c59f12750046))

## [0.4.11](https://github.com/ing-bank/lion/compare/@lion/form@0.4.10...@lion/form@0.4.11) (2020-02-10)

**Note:** Version bump only for package @lion/form

## [0.4.10](https://github.com/ing-bank/lion/compare/@lion/form@0.4.9...@lion/form@0.4.10) (2020-02-06)

**Note:** Version bump only for package @lion/form

## [0.4.9](https://github.com/ing-bank/lion/compare/@lion/form@0.4.8...@lion/form@0.4.9) (2020-02-06)

**Note:** Version bump only for package @lion/form

## [0.4.8](https://github.com/ing-bank/lion/compare/@lion/form@0.4.7...@lion/form@0.4.8) (2020-02-06)

**Note:** Version bump only for package @lion/form

## [0.4.7](https://github.com/ing-bank/lion/compare/@lion/form@0.4.6...@lion/form@0.4.7) (2020-02-05)

**Note:** Version bump only for package @lion/form

## [0.4.6](https://github.com/ing-bank/lion/compare/@lion/form@0.4.5...@lion/form@0.4.6) (2020-02-05)

**Note:** Version bump only for package @lion/form

## [0.4.5](https://github.com/ing-bank/lion/compare/@lion/form@0.4.4...@lion/form@0.4.5) (2020-02-03)

**Note:** Version bump only for package @lion/form

## [0.4.4](https://github.com/ing-bank/lion/compare/@lion/form@0.4.3...@lion/form@0.4.4) (2020-01-23)

### Bug Fixes

- move demos to form-system to avoid circular dependencies ([ddd1a72](https://github.com/ing-bank/lion/commit/ddd1a72ba752c9798885d9c8cd7706a69ed3abb2))
- update links in stories ([0c53b1d](https://github.com/ing-bank/lion/commit/0c53b1d4bb4fa51820656bacfc2aece653d03182))

## [0.4.3](https://github.com/ing-bank/lion/compare/@lion/form@0.4.2...@lion/form@0.4.3) (2020-01-23)

**Note:** Version bump only for package @lion/form

## [0.4.2](https://github.com/ing-bank/lion/compare/@lion/form@0.4.1...@lion/form@0.4.2) (2020-01-20)

**Note:** Version bump only for package @lion/form

## [0.4.1](https://github.com/ing-bank/lion/compare/@lion/form@0.4.0...@lion/form@0.4.1) (2020-01-17)

### Bug Fixes

- update storybook and use main.js ([e61e0b9](https://github.com/ing-bank/lion/commit/e61e0b938ff72cc18cc0b3aa1560f2cece0c9fe6))

# [0.4.0](https://github.com/ing-bank/lion/compare/@lion/form@0.3.14...@lion/form@0.4.0) (2020-01-13)

### Features

- improved storybook demos ([89b835a](https://github.com/ing-bank/lion/commit/89b835a79998c45a28093de01f69216c35009a40))

## [0.3.14](https://github.com/ing-bank/lion/compare/@lion/form@0.3.13...@lion/form@0.3.14) (2020-01-08)

**Note:** Version bump only for package @lion/form

## [0.3.13](https://github.com/ing-bank/lion/compare/@lion/form@0.3.12...@lion/form@0.3.13) (2019-12-16)

**Note:** Version bump only for package @lion/form

## [0.3.12](https://github.com/ing-bank/lion/compare/@lion/form@0.3.11...@lion/form@0.3.12) (2019-12-13)

**Note:** Version bump only for package @lion/form

## [0.3.11](https://github.com/ing-bank/lion/compare/@lion/form@0.3.10...@lion/form@0.3.11) (2019-12-11)

**Note:** Version bump only for package @lion/form

## [0.3.10](https://github.com/ing-bank/lion/compare/@lion/form@0.3.9...@lion/form@0.3.10) (2019-12-06)

### Bug Fixes

- **form:** event order of reset and submit ([190ba38](https://github.com/ing-bank/lion/commit/190ba3854a6a031f996e77a7c2ee4cbf851fecbb))

## [0.3.9](https://github.com/ing-bank/lion/compare/@lion/form@0.3.8...@lion/form@0.3.9) (2019-12-04)

**Note:** Version bump only for package @lion/form

## [0.3.8](https://github.com/ing-bank/lion/compare/@lion/form@0.3.7...@lion/form@0.3.8) (2019-12-03)

### Bug Fixes

- let lerna publish fixed versions ([bc7448c](https://github.com/ing-bank/lion/commit/bc7448c694deb3c05fd3d083a9acb5365b26b7ab))

## [0.3.7](https://github.com/ing-bank/lion/compare/@lion/form@0.3.6...@lion/form@0.3.7) (2019-12-02)

### Bug Fixes

- use strict versions to get correct deps on older versions ([8645c13](https://github.com/ing-bank/lion/commit/8645c13b1d77e488713f2e5e0e4e00c4d30ea1ee))

## [0.3.6](https://github.com/ing-bank/lion/compare/@lion/form@0.3.5...@lion/form@0.3.6) (2019-12-01)

**Note:** Version bump only for package @lion/form

## [0.3.5](https://github.com/ing-bank/lion/compare/@lion/form@0.3.4...@lion/form@0.3.5) (2019-11-28)

**Note:** Version bump only for package @lion/form

## [0.3.4](https://github.com/ing-bank/lion/compare/@lion/form@0.3.3...@lion/form@0.3.4) (2019-11-27)

**Note:** Version bump only for package @lion/form

## [0.3.3](https://github.com/ing-bank/lion/compare/@lion/form@0.3.2...@lion/form@0.3.3) (2019-11-27)

**Note:** Version bump only for package @lion/form

## [0.3.2](https://github.com/ing-bank/lion/compare/@lion/form@0.3.1...@lion/form@0.3.2) (2019-11-26)

**Note:** Version bump only for package @lion/form

## [0.3.1](https://github.com/ing-bank/lion/compare/@lion/form@0.3.0...@lion/form@0.3.1) (2019-11-22)

**Note:** Version bump only for package @lion/form

# [0.3.0](https://github.com/ing-bank/lion/compare/@lion/form@0.2.1...@lion/form@0.3.0) (2019-11-18)

### Features

- finalize validation and adopt it everywhere ([396deb2](https://github.com/ing-bank/lion/commit/396deb2e3b4243f102a5c98e9b0518fa0f31a6b1))

## [0.2.1](https://github.com/ing-bank/lion/compare/@lion/form@0.2.0...@lion/form@0.2.1) (2019-11-15)

**Note:** Version bump only for package @lion/form

# [0.2.0](https://github.com/ing-bank/lion/compare/@lion/form@0.1.73...@lion/form@0.2.0) (2019-11-13)

### Features

- remove all deprecations from lion ([66d3d39](https://github.com/ing-bank/lion/commit/66d3d390aebeaa61b6effdea7d5f7eea0e89c894))

## [0.1.73](https://github.com/ing-bank/lion/compare/@lion/form@0.1.72...@lion/form@0.1.73) (2019-11-12)

**Note:** Version bump only for package @lion/form

## [0.1.72](https://github.com/ing-bank/lion/compare/@lion/form@0.1.71...@lion/form@0.1.72) (2019-11-06)

**Note:** Version bump only for package @lion/form

## [0.1.71](https://github.com/ing-bank/lion/compare/@lion/form@0.1.70...@lion/form@0.1.71) (2019-11-01)

**Note:** Version bump only for package @lion/form

## [0.1.70](https://github.com/ing-bank/lion/compare/@lion/form@0.1.69...@lion/form@0.1.70) (2019-10-25)

**Note:** Version bump only for package @lion/form

## [0.1.69](https://github.com/ing-bank/lion/compare/@lion/form@0.1.68...@lion/form@0.1.69) (2019-10-23)

**Note:** Version bump only for package @lion/form

## [0.1.68](https://github.com/ing-bank/lion/compare/@lion/form@0.1.67...@lion/form@0.1.68) (2019-10-23)

**Note:** Version bump only for package @lion/form

## [0.1.67](https://github.com/ing-bank/lion/compare/@lion/form@0.1.66...@lion/form@0.1.67) (2019-10-21)

**Note:** Version bump only for package @lion/form

## [0.1.66](https://github.com/ing-bank/lion/compare/@lion/form@0.1.65...@lion/form@0.1.66) (2019-10-14)

**Note:** Version bump only for package @lion/form

## [0.1.65](https://github.com/ing-bank/lion/compare/@lion/form@0.1.64...@lion/form@0.1.65) (2019-10-11)

**Note:** Version bump only for package @lion/form

## [0.1.64](https://github.com/ing-bank/lion/compare/@lion/form@0.1.63...@lion/form@0.1.64) (2019-10-11)

**Note:** Version bump only for package @lion/form

## [0.1.63](https://github.com/ing-bank/lion/compare/@lion/form@0.1.62...@lion/form@0.1.63) (2019-10-09)

**Note:** Version bump only for package @lion/form

## [0.1.62](https://github.com/ing-bank/lion/compare/@lion/form@0.1.61...@lion/form@0.1.62) (2019-10-07)

**Note:** Version bump only for package @lion/form

## [0.1.61](https://github.com/ing-bank/lion/compare/@lion/form@0.1.60...@lion/form@0.1.61) (2019-09-30)

**Note:** Version bump only for package @lion/form

## [0.1.60](https://github.com/ing-bank/lion/compare/@lion/form@0.1.59...@lion/form@0.1.60) (2019-09-27)

**Note:** Version bump only for package @lion/form

## [0.1.59](https://github.com/ing-bank/lion/compare/@lion/form@0.1.58...@lion/form@0.1.59) (2019-09-25)

**Note:** Version bump only for package @lion/form

## [0.1.58](https://github.com/ing-bank/lion/compare/@lion/form@0.1.57...@lion/form@0.1.58) (2019-09-20)

**Note:** Version bump only for package @lion/form

## [0.1.57](https://github.com/ing-bank/lion/compare/@lion/form@0.1.56...@lion/form@0.1.57) (2019-09-19)

**Note:** Version bump only for package @lion/form

## [0.1.56](https://github.com/ing-bank/lion/compare/@lion/form@0.1.55...@lion/form@0.1.56) (2019-09-13)

**Note:** Version bump only for package @lion/form

## [0.1.55](https://github.com/ing-bank/lion/compare/@lion/form@0.1.54...@lion/form@0.1.55) (2019-08-23)

**Note:** Version bump only for package @lion/form

## [0.1.54](https://github.com/ing-bank/lion/compare/@lion/form@0.1.53...@lion/form@0.1.54) (2019-08-21)

**Note:** Version bump only for package @lion/form

## [0.1.53](https://github.com/ing-bank/lion/compare/@lion/form@0.1.52...@lion/form@0.1.53) (2019-08-17)

**Note:** Version bump only for package @lion/form

## [0.1.52](https://github.com/ing-bank/lion/compare/@lion/form@0.1.51...@lion/form@0.1.52) (2019-08-15)

**Note:** Version bump only for package @lion/form

## [0.1.51](https://github.com/ing-bank/lion/compare/@lion/form@0.1.50...@lion/form@0.1.51) (2019-08-15)

**Note:** Version bump only for package @lion/form

## [0.1.50](https://github.com/ing-bank/lion/compare/@lion/form@0.1.49...@lion/form@0.1.50) (2019-08-14)

### Bug Fixes

- **form:** sync submit and reset events instead of delegating ([5534369](https://github.com/ing-bank/lion/commit/5534369))

## [0.1.49](https://github.com/ing-bank/lion/compare/@lion/form@0.1.48...@lion/form@0.1.49) (2019-08-07)

**Note:** Version bump only for package @lion/form

## [0.1.48](https://github.com/ing-bank/lion/compare/@lion/form@0.1.47...@lion/form@0.1.48) (2019-08-07)

**Note:** Version bump only for package @lion/form

## [0.1.47](https://github.com/ing-bank/lion/compare/@lion/form@0.1.46...@lion/form@0.1.47) (2019-07-30)

**Note:** Version bump only for package @lion/form

## [0.1.46](https://github.com/ing-bank/lion/compare/@lion/form@0.1.45...@lion/form@0.1.46) (2019-07-30)

**Note:** Version bump only for package @lion/form

## [0.1.45](https://github.com/ing-bank/lion/compare/@lion/form@0.1.44...@lion/form@0.1.45) (2019-07-29)

**Note:** Version bump only for package @lion/form

## [0.1.44](https://github.com/ing-bank/lion/compare/@lion/form@0.1.43...@lion/form@0.1.44) (2019-07-25)

**Note:** Version bump only for package @lion/form

## [0.1.43](https://github.com/ing-bank/lion/compare/@lion/form@0.1.42...@lion/form@0.1.43) (2019-07-24)

**Note:** Version bump only for package @lion/form

## [0.1.42](https://github.com/ing-bank/lion/compare/@lion/form@0.1.41...@lion/form@0.1.42) (2019-07-24)

**Note:** Version bump only for package @lion/form

## [0.1.41](https://github.com/ing-bank/lion/compare/@lion/form@0.1.40...@lion/form@0.1.41) (2019-07-23)

**Note:** Version bump only for package @lion/form

## [0.1.40](https://github.com/ing-bank/lion/compare/@lion/form@0.1.39...@lion/form@0.1.40) (2019-07-23)

**Note:** Version bump only for package @lion/form

## [0.1.39](https://github.com/ing-bank/lion/compare/@lion/form@0.1.38...@lion/form@0.1.39) (2019-07-23)

**Note:** Version bump only for package @lion/form

## [0.1.38](https://github.com/ing-bank/lion/compare/@lion/form@0.1.37...@lion/form@0.1.38) (2019-07-22)

**Note:** Version bump only for package @lion/form

## [0.1.37](https://github.com/ing-bank/lion/compare/@lion/form@0.1.36...@lion/form@0.1.37) (2019-07-19)

**Note:** Version bump only for package @lion/form

## [0.1.36](https://github.com/ing-bank/lion/compare/@lion/form@0.1.35...@lion/form@0.1.36) (2019-07-19)

**Note:** Version bump only for package @lion/form

## [0.1.35](https://github.com/ing-bank/lion/compare/@lion/form@0.1.34...@lion/form@0.1.35) (2019-07-18)

**Note:** Version bump only for package @lion/form

## [0.1.34](https://github.com/ing-bank/lion/compare/@lion/form@0.1.33...@lion/form@0.1.34) (2019-07-17)

**Note:** Version bump only for package @lion/form

## [0.1.33](https://github.com/ing-bank/lion/compare/@lion/form@0.1.32...@lion/form@0.1.33) (2019-07-16)

**Note:** Version bump only for package @lion/form

## [0.1.32](https://github.com/ing-bank/lion/compare/@lion/form@0.1.31...@lion/form@0.1.32) (2019-07-16)

**Note:** Version bump only for package @lion/form

## [0.1.31](https://github.com/ing-bank/lion/compare/@lion/form@0.1.30...@lion/form@0.1.31) (2019-07-15)

**Note:** Version bump only for package @lion/form

## [0.1.30](https://github.com/ing-bank/lion/compare/@lion/form@0.1.29...@lion/form@0.1.30) (2019-07-15)

**Note:** Version bump only for package @lion/form

## [0.1.29](https://github.com/ing-bank/lion/compare/@lion/form@0.1.28...@lion/form@0.1.29) (2019-07-09)

**Note:** Version bump only for package @lion/form

## [0.1.28](https://github.com/ing-bank/lion/compare/@lion/form@0.1.27...@lion/form@0.1.28) (2019-07-04)

**Note:** Version bump only for package @lion/form

## [0.1.27](https://github.com/ing-bank/lion/compare/@lion/form@0.1.26...@lion/form@0.1.27) (2019-07-02)

**Note:** Version bump only for package @lion/form

## [0.1.26](https://github.com/ing-bank/lion/compare/@lion/form@0.1.25...@lion/form@0.1.26) (2019-07-02)

**Note:** Version bump only for package @lion/form

## [0.1.25](https://github.com/ing-bank/lion/compare/@lion/form@0.1.24...@lion/form@0.1.25) (2019-06-27)

**Note:** Version bump only for package @lion/form

## [0.1.24](https://github.com/ing-bank/lion/compare/@lion/form@0.1.23...@lion/form@0.1.24) (2019-06-24)

**Note:** Version bump only for package @lion/form

## [0.1.23](https://github.com/ing-bank/lion/compare/@lion/form@0.1.22...@lion/form@0.1.23) (2019-06-20)

**Note:** Version bump only for package @lion/form

## [0.1.22](https://github.com/ing-bank/lion/compare/@lion/form@0.1.21...@lion/form@0.1.22) (2019-06-18)

**Note:** Version bump only for package @lion/form

## [0.1.21](https://github.com/ing-bank/lion/compare/@lion/form@0.1.20...@lion/form@0.1.21) (2019-06-06)

**Note:** Version bump only for package @lion/form

## [0.1.20](https://github.com/ing-bank/lion/compare/@lion/form@0.1.19...@lion/form@0.1.20) (2019-06-04)

**Note:** Version bump only for package @lion/form

## [0.1.19](https://github.com/ing-bank/lion/compare/@lion/form@0.1.18...@lion/form@0.1.19) (2019-05-31)

**Note:** Version bump only for package @lion/form

## [0.1.18](https://github.com/ing-bank/lion/compare/@lion/form@0.1.17...@lion/form@0.1.18) (2019-05-31)

**Note:** Version bump only for package @lion/form

## [0.1.17](https://github.com/ing-bank/lion/compare/@lion/form@0.1.16...@lion/form@0.1.17) (2019-05-29)

**Note:** Version bump only for package @lion/form

## [0.1.16](https://github.com/ing-bank/lion/compare/@lion/form@0.1.15...@lion/form@0.1.16) (2019-05-29)

**Note:** Version bump only for package @lion/form

## [0.1.15](https://github.com/ing-bank/lion/compare/@lion/form@0.1.14...@lion/form@0.1.15) (2019-05-24)

**Note:** Version bump only for package @lion/form

## [0.1.14](https://github.com/ing-bank/lion/compare/@lion/form@0.1.13...@lion/form@0.1.14) (2019-05-22)

**Note:** Version bump only for package @lion/form

## [0.1.13](https://github.com/ing-bank/lion/compare/@lion/form@0.1.12...@lion/form@0.1.13) (2019-05-21)

**Note:** Version bump only for package @lion/form

## [0.1.12](https://github.com/ing-bank/lion/compare/@lion/form@0.1.11...@lion/form@0.1.12) (2019-05-17)

**Note:** Version bump only for package @lion/form

## [0.1.11](https://github.com/ing-bank/lion/compare/@lion/form@0.1.10...@lion/form@0.1.11) (2019-05-16)

**Note:** Version bump only for package @lion/form

## [0.1.10](https://github.com/ing-bank/lion/compare/@lion/form@0.1.9...@lion/form@0.1.10) (2019-05-16)

**Note:** Version bump only for package @lion/form

## [0.1.9](https://github.com/ing-bank/lion/compare/@lion/form@0.1.8...@lion/form@0.1.9) (2019-05-15)

### Bug Fixes

- **form:** native submit event should not trigger an error ([f2c4433](https://github.com/ing-bank/lion/commit/f2c4433))

## [0.1.8](https://github.com/ing-bank/lion/compare/@lion/form@0.1.7...@lion/form@0.1.8) (2019-05-13)

**Note:** Version bump only for package @lion/form

## [0.1.7](https://github.com/ing-bank/lion/compare/@lion/form@0.1.6...@lion/form@0.1.7) (2019-05-13)

### Bug Fixes

- add prepublish step to make links absolute for npm docs ([9f2c4f6](https://github.com/ing-bank/lion/commit/9f2c4f6))

## [0.1.6](https://github.com/ing-bank/lion/compare/@lion/form@0.1.5...@lion/form@0.1.6) (2019-05-08)

**Note:** Version bump only for package @lion/form

## [0.1.5](https://github.com/ing-bank/lion/compare/@lion/form@0.1.4...@lion/form@0.1.5) (2019-05-07)

**Note:** Version bump only for package @lion/form

## [0.1.4](https://github.com/ing-bank/lion/compare/@lion/form@0.1.3...@lion/form@0.1.4) (2019-04-29)

**Note:** Version bump only for package @lion/form

## [0.1.3](https://github.com/ing-bank/lion/compare/@lion/form@0.1.2...@lion/form@0.1.3) (2019-04-28)

### Bug Fixes

- update storybook/linting; adjust story labels, eslint ignores ([8d96f84](https://github.com/ing-bank/lion/commit/8d96f84))

## [0.1.2](https://github.com/ing-bank/lion/compare/@lion/form@0.1.1...@lion/form@0.1.2) (2019-04-27)

**Note:** Version bump only for package @lion/form

## [0.1.1](https://github.com/ing-bank/lion/compare/@lion/form@0.1.0...@lion/form@0.1.1) (2019-04-26)

### Bug Fixes

- add missing files to npm packages ([0e3ca17](https://github.com/ing-bank/lion/commit/0e3ca17))

# 0.1.0 (2019-04-26)

### Bug Fixes

- cycle dependencies by adding form-system package ([38dcca9](https://github.com/ing-bank/lion/commit/38dcca9))

### Features

- release inital public lion version ([ec8da8f](https://github.com/ing-bank/lion/commit/ec8da8f))
