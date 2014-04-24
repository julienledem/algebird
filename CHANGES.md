# Algebird #

### Version 0.6.0 ###
* make constructors for SpaceSaver subclasses public so that deserializers..: https://github.com/twitter/algebird/pull/289
* Restoring optimized SketchMapMonoid#sumOption: https://github.com/twitter/algebird/pull/293
* Newer caliper hll benchmark: https://github.com/twitter/algebird/pull/297
* hll optimization: https://github.com/twitter/algebird/pull/299
* Optimize the storage backend used in sketch map: https://github.com/twitter/algebird/pull/301
* migrate async summers from Summingbird: https://github.com/twitter/algebird/pull/296
* add sumOption to EventuallySemiGroup: https://github.com/twitter/algebird/pull/306
* Heavyhitters no longer attempts lazy storage in SketchMap: https://github.com/twitter/algebird/pull/305
* Async Maps performance improvements: https://github.com/twitter/algebird/pull/302
* Make the AsyncListSum be immutable again: https://github.com/twitter/algebird/pull/309

### Version 0.5.0 ###
* Remove handling that doesn't seem needed/wanted for longs: https://github.com/twitter/algebird/pull/287
* Add average() for DecayedValue: https://github.com/twitter/algebird/pull/286
* SketchMapParams can support being constructed with both width/depth and eps/delta: https://github.com/twitter/algebird/pull/285
* undo the undo of the interval fixes: https://github.com/twitter/algebird/pull/283
* Fix priority queue bug found by scalacheck: https://github.com/twitter/algebird/pull/280
* Adds type parameters to Intersection for more precision: https://github.com/twitter/algebird/pull/279
* Make resolver consistent with scalding: https://github.com/twitter/algebird/pull/276
* remove Math use in test: https://github.com/twitter/algebird/pull/275
* Remove extends function from algebird: https://github.com/twitter/algebird/pull/274
* remove unnecessary implicit requirement: https://github.com/twitter/algebird/pull/272
* Fix SketchMapMonoid zero: https://github.com/twitter/algebird/pull/269
* Make SketchMapMonoid params public: https://github.com/twitter/algebird/pull/265
* Add Predecessible and methods to Interval: https://github.com/twitter/algebird/pull/262
* Implement StreamSummary data structure for finding frequent/top-k items: https://github.com/twitter/algebird/pull/259

### Version 0.4.0 ###
* Make SketchMap1 the only SketchMap implementation: https://github.com/twitter/algebird/pull/256
* Use semigroup in StateWithError: https://github.com/twitter/algebird/pull/255
* Don't iterate through everything in unit monoid: https://github.com/twitter/algebird/pull/253
* Factor as much logic as possible into SketchmapMonoid1: https://github.com/twitter/algebird/pull/251
* Moving Trampoline flatMap implementation into trait: https://github.com/twitter/algebird/pull/249
* Integrate Caliper: https://github.com/twitter/algebird/pull/248
* Adds append method to MonoidAggregator and RingAggregator: https://github.com/twitter/algebird/pull/246
* Make the map monoid more performant for mutable maps: https://github.com/twitter/algebird/pull/245
* Make BFHash take on non negative values only: https://github.com/twitter/algebird/pull/243
* Fixed DecayedValue: https://github.com/twitter/algebird/pull/238
* Updated scaladoc to 0.3.0: https://github.com/twitter/algebird/pull/237
* Add Incrementable and tests: https://github.com/twitter/algebird/pull/234
* Updates sbt runner: https://github.com/twitter/algebird/pull/232
* Upgrade sbt, specs, add a build.properties, and bump travis's target: https://github.com/twitter/algebird/pull/231

### Version 0.3.1 ###
* Make a field transient in BloomFilter serialization: https://github.com/twitter/algebird/pull/209
* Add the TunnelMonoid to Util (like async function monoid): https://github.com/twitter/algebird/pull/213
* Make DecayedValueMonoid a class: https://github.com/twitter/algebird/pull/223
* SketchMap performance improvements: https://github.com/twitter/algebird/pull/227
* Add the Option group: https://github.com/twitter/algebird/pull/230
* Add Successible Typeclass: https://github.com/twitter/algebird/pull/234
* sumOption support on generated tuple Semigroups: https://github.com/twitter/algebird/pull/242

### Version 0.3.0 ###
* Optimize lots of the Monoids/Semigroups when summing many items: see Semigroup.sumOption https://github.com/twitter/algebird/pull/206
* Add many Aggregators for more convenient aggregation: https://github.com/twitter/algebird/pull/194
* Aggregators compose: https://github.com/twitter/algebird/pull/188
* Added scala.collection.Map (not just immutable.Map) algebras: https://github.com/twitter/algebird/pull/199
* Added Boolean monoids (Or and And): https://github.com/twitter/algebird/pull/198

### Version 0.2.0 ###

* Adds algebird-bijection module: https://github.com/twitter/algebird/pull/181
* Build cleanups: https://github.com/twitter/algebird/pull/180
* MapAlgebra.sparseEquiv: https://github.com/twitter/algebird/pull/182
* Remove isNonZero from Semigroup, add to Monoid: https://github.com/twitter/algebird/pull/183
* add MapAlgebra.mergeLookup: https://github.com/twitter/algebird/pull/185

### Version 0.1.13 ###
* Adds QTree monoid for range queries

### Version 0.1.12 ###
* Adds hashing trick monoid for dimensionality reduction

### Version 0.1.10 ###
* Fix compiler flag issue

### Version 0.1.9 ###

* Build `algebird` against scala 2.9.2 and 2.10.0
* `algebird-util` with Future and Try algebras.

### Version 0.1.8 ###

* Break out `algebird-core` and `algebird-test` into separate jars

### Version 0.1.7 ###

* SummingQueue works with capacity of 0, just passes through
* adds compressed bitset (RichCBitSet)
* Add `BFSparse`
* Heavy hitters in countminsketch
* Monad typeclass

### Version 0.1.6 ###

* Adds publishing pom.
* Add SummingQueue
* rename Cassandra's MurmurHash.

### Version 0.1.5 ###
* Make Metric serializable
* JMap uses Semigroup

### Version 0.1.4 ###
* Count-min-sketch (with Monoid)
* Added Bloom Filter (with Monoid)
* HyperLogLog now uses Murmur128 (should be faster)
* Max/Min/First/Last Monoids
* VectorSpace trait (implementations for Maps/Vector)
* DecayedVector for efficient exponential moving average on vectors
* Metric trait
* Approximate[Numeric]/Boolean to track error in approximations
* Adds Semigroup and implicits for usual primitives and collections
* Fixes EitherMonoid to have a zero
* Add MinPlus algebra for shortest path calculations
* Lots of code cleanups

### Version 0.1.2 ###
* Improves speed of HyperLogLog.
* Refactoring of RightFolded Monoid

### Version 0.1.1 ###
* Added Moments monoid for first 5 moments
* Improved HyperLogLogMonoid (less memory usage, added intersections)

### Version 0.1.0 ###
* Moved code over from Scalding.
