# Change Log

All notable changes to this project will be documented in this file.
See [Conventional Commits](https://conventionalcommits.org) for commit guidelines.

<a name="0.7.0"></a>

## [0.7.0](https://github.com/timhagn/gatsby-background-image) (2019-05-28)

**feat:** Added possibility to work with multiple stacked background-images.

## [0.6.2](https://github.com/timhagn/gatsby-background-image) (2019-05-19)

**merge:** Merged PR from @seangabe fixing TypeDefs.

## [0.6.1](https://github.com/timhagn/gatsby-background-image) (2019-05-15)

**fix / feat:** Fixed some quirks with transitions, add integration tests.

## [0.6.0](https://github.com/timhagn/gatsby-background-image) (2019-05-14)

**feat:** Split packages in `gatsby-background-image` & `gatsby-background-image-es5`.

## [0.5.9](https://github.com/timhagn/gatsby-background-image) (2019-05-13)

**quickfix:** Changed `@babel/runtime-corejs3` back to `@babel/runtime`.

## [0.5.8](https://github.com/timhagn/gatsby-background-image) (2019-05-13)

**fix:** With `@babel/runtime-corejs3` package size exploded, so just targeted
specific function missing in IE 11 and exchanged `Array.from` with
`Array.prototype.slice.call` and `Array.find` with its `Array.reduce` equivalent.

## [0.5.7](https://github.com/timhagn/gatsby-background-image) (2019-05-12)

**fix:** Removed `@babel-polyfill` and went with `@babel/runtime-corejs3`.

## [0.5.6](https://github.com/timhagn/gatsby-background-image) (2019-05-07)

**fix:** Added some workarounds and `@babel-polyfill` for IE11 compatibility,
reintroduced `imageRef.src` as fallback for browsers without `currentSrc`.

## [0.5.5](https://github.com/timhagn/gatsby-background-image) (2019-05-07)

**fix:** Replaced Math.random() "hash" generation with an implementation of
Java's hashCode() function on either current `srcSet` or given `className`.

## [0.5.4](https://github.com/timhagn/gatsby-background-image) (2019-05-07)

**feat / fix:** Added a componentClassCache to prevent duplicate render with
different images.

## [0.5.3](https://github.com/timhagn/gatsby-background-image) (2019-05-04)

**feat:** Contribution of TypeScript definitions.

## [0.5.2](https://github.com/timhagn/gatsby-background-image) (2019-05-02)

**fix:** Added isVisible to activatePictureRef() props (page change / cached).

## [0.5.1](https://github.com/timhagn/gatsby-background-image) (2019-05-02)

**fix:** Added activatePictureRef() to really only load critical or visible images.

## [0.5.0](https://github.com/timhagn/gatsby-background-image) (2019-05-01)

**deprecation / refactor / fix / feat / doc:**

- `_depr` was added to classes generated by adding classId.
- `<BackgroundImage />` fixed & fluid branches were simplified to one return value.
- As the transitions still didn't work, a "micro fixed state machine (mFSM)" was
  integrated. Tests were refactored, mocks and setup moved to their own file.
- `isMounted` was removed in favor of setting `imageRef.onload` to `null` on
  `componentWillUnmount`.
- SSR tests were added.
- Code Coverage was pushed to 100%.
- codecov was added to CircleCI build and badge added to README.

## [0.4.3](https://github.com/timhagn/gatsby-background-image) (2019-04-29)

**fix:** Fixed transitions for the moment for issue #26.

## [0.4.2](https://github.com/timhagn/gatsby-background-image) (2019-04-28)

**doc / feat:** Changed babel behavior from @babel/polyfill to new
core-js/stable & updated README.md.

## [0.4.1](https://github.com/timhagn/gatsby-background-image) (2019-04-25)

**fix:** Called extracted intersectionListener function instead of passing it.

## [0.4.0](https://github.com/timhagn/gatsby-background-image) (2019-04-25)

**feat:** Get feature par with gatsby-image again (add `durationFadeIn` &
`crossOrigin` props), update tests accordingly. Refactor anonymous IO callback
to intersectionlistener(), more tests.

## [0.3.6](https://github.com/timhagn/gatsby-background-image) (2019-04-20)

**feat / fix:** Merge #25, fix test errors.

## [0.3.5](https://github.com/timhagn/gatsby-background-image) (2019-04-14)

**fix:** Duplicate propTypes names to gbiPropTypes array.

## [0.3.4](https://github.com/timhagn/gatsby-background-image) (2019-04-16)

**fix / feat:** Fix behavior when changing fluid / fixed image props (didn't
recreate imageRef before). Add possibility for passing `soft` to `fadeIn` to
"force" fading in and image even if it is in cache.

## [0.3.3](https://github.com/timhagn/gatsby-background-image) (2019-04-15)

**doc / feat:** Remove TODO for object-fit / -position (superfluous); specify
how to use `intersection-observer` polyfill. Sync IO with `gatsby-image`.

## [0.3.2](https://github.com/timhagn/gatsby-background-image) (2019-04-14)

**fix:** Add title attribute.

## [0.3.1](https://github.com/timhagn/gatsby-background-image) (2019-04-14)

**feat:** Add stripRemainingProps() to safely add ARIA or other attributes.

## [0.3.0](https://github.com/timhagn/gatsby-background-image) (2019-04-12)

**fix / feat:** Add most changes from issue #20 (styling), fixes issue #22.

## [0.2.9](https://github.com/timhagn/gatsby-background-image) (2019-04-05)

**fix:** Change build to ES5.

## [0.2.8](https://github.com/timhagn/gatsby-background-image) (2019-04-05)

**fix:** Add id as prop, fix some issues with transitions.

## [0.2.8-beta](https://github.com/timhagn/gatsby-background-image) (2019-03-13)

**fix:** Add some props, parse more backgroundStyles.

## [0.2.5](https://github.com/timhagn/gatsby-background-image) (2019-03-13)

**fix:** Add picture wrapper in image creation.

## [0.2.0](https://github.com/timhagn/gatsby-background-image) (2018-12-13)

**feat:** Remove superfluous placeholder images, tracedSVG working.

## [0.1.0](https://github.com/timhagn/gatsby-background-image) (2018-12-13)

**Initial commit:** Tests running and module working.
