# Version 0.3

* BREAKING: Renamed module `Exinst.Singletons` to  `Exinst`.

* BREAKING: The `Exinst.Instances.Base` module is gone. The `base` instances are
  now exported from `Exinst`.

* Add `Dict0`.

* Re-export `Constraint` from `base`.

* Add `Dict{0,2,3,4}` instances for `Bool`.

* Add `GHC.Generics.Generic` support for `Some{1,2,3,4}`. This only works for
  indexes with `PEnum` and `PBounded` instances.

* Added tests.

* Added `Test.QuickCheck.Arbitrary` instances for `Some{1,2,3,4}` in
  `Exinst.Instances.QuickCheck`. These instances and their dependency on
  `QuickCheck` can be toggled with the `quickcheck` Cabal flag.

* Added `Data.Aeson.{FromJSON,ToJSON}` instances for `Some{1,2,3,4}` in
  `Exinst.Instances.Aeson`. These instances and their dependency on
  `aeson` can be toggled with the `aeson` Cabal flag. These instances used to
  exist in now-deprecated the `exinst-aeson` package, and are compatible with
  them.

* Added `Bytes.Serial.Serial` instances for `Some{1,2,3,4}` in
  `Exinst.Instances.Bytes`. These instances and their dependency on `bytes` can
  be toggled with the `bytes` Cabal flag. These instances used to exist in
  now-deprecated the `exinst-bytes` package, and are compatible with them.

* Added `Control.DeepSeq.NFData` instances for `Some{1,2,3,4}` in
  `Exinst.Instances.DeepSeq`. These instances and their dependency on `deepseq`
  can be toggled with the `deepseq` Cabal flag. These instances used to exist in
  now-deprecated the `exinst-deepseq` package, and are compatible with them.

* Added `Data.Hashable.Hashable` instances for `Some{1,2,3,4}` in
  `Exinst.Instances.DeepSeq`. These instances and their dependency on `hashable`
  can be toggled with the `hashable` Cabal flag. These instances used to exist
  in now-deprecated the `exinst-hashable` package, and are compatible with them.


# Version 0.2

* Depend on `singletons-2.2`, which means `KProxy` is gone.

* Add `_Some{1,2,3,4}` prisms.

* Add `Dict1` instance for `Bool`.

* Add `some{1,2,3,4}SingRep`.

* Thanks to Sandy Maguire for having contributed to this release.


# Version 0.1.2

* Export the `Some{1,2,3,4}` constructors.

* Make all the fields in `Some{1,2,3,4}` strict.

* Relax upper bound on `base`, `singletons`, `constraints`.

* Re-export `Dict(Dict)` from `constraints`.


# Version 0.1.1

* Relax upper bound on `singletons` dependency.

* `withSome{1,2,3,4}Sing` brings `SingI` instances to scope.

* Generalized the `(* -> Constraint)` parameter in `Dict{1,2,3,4}`
  to `(k -> Constraint)`.


# Version 0.1

* Initial release.
