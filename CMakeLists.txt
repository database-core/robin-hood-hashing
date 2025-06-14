cmake_minimum_required(VERSION 3.14)
project(robin_hood_hashing)

set(CMAKE_CXX_STANDARD 14)

include_directories(src/include)
include_directories(src/test/app)
include_directories(src/test/app/fmt)
include_directories(src/test/app/hash)
include_directories(src/test/thirdparty)
include_directories(src/test/thirdparty/doctest)
include_directories(src/test/thirdparty/nanobench)
include_directories(src/test/unit)

add_executable(robin_hood_hashing
        src/external_cmake/myproject.cpp
        src/include/robin_hood.h
        src/test/app/fmt/bin.h
        src/test/app/fmt/hex.h
        src/test/app/fmt/mup.cpp
        src/test/app/fmt/mup.h
        src/test/app/fmt/streamstate.cpp
        src/test/app/fmt/streamstate.h
        src/test/app/hash/Bad.h
        src/test/app/hash/FNV1a.h
        src/test/app/hash/Identity.h
        src/test/app/avalanche.h
        src/test/app/benchmark.cpp
        src/test/app/benchmark.h
        src/test/app/checksum.h
        src/test/app/Counter.cpp
        src/test/app/Counter.h
        src/test/app/counter_defaults.h
        src/test/app/CtorDtorVerifier.cpp
        src/test/app/CtorDtorVerifier.h
        src/test/app/doctest.h
        src/test/app/geomean.h
        src/test/app/nanobench.cpp
        src/test/app/PerformanceCounters.cpp
        src/test/app/PerformanceCounters.h
        src/test/app/randomseed.cpp
        src/test/app/randomseed.h
        src/test/app/sfc64.h
        src/test/thirdparty/doctest/doctest.h
        src/test/thirdparty/nanobench/nanobench.h
        src/test/unit/bench_copy_iterators.cpp
        src/test/unit/bench_distinctness.cpp
        src/test/unit/bench_find_random.cpp
        src/test/unit/bench_hash_int.cpp
        src/test/unit/bench_hash_string.cpp
        src/test/unit/bench_iterate.cpp
        src/test/unit/bench_quick_overall_map.cpp
        src/test/unit/bench_quick_overall_set.cpp
        src/test/unit/bench_random_insert_erase.cpp
        src/test/unit/bench_swap.cpp
        src/test/unit/count_ctor_dtor.cpp
        src/test/unit/count_ctor_dtor_1.cpp
        src/test/unit/count_find_random.cpp
        src/test/unit/count_one_emplace.cpp
        src/test/unit/count_random_insert_erase.cpp
        src/test/unit/fuzz_insert_erase.cpp
        src/test/unit/include_only.cpp
        src/test/unit/include_only.h
        src/test/unit/main.cpp
        src/test/unit/optimize_avalanche.cpp
        src/test/unit/show_hash.cpp
        src/test/unit/unit_addOrFree.cpp
        src/test/unit/unit_assertNotNull.cpp
        src/test/unit/unit_assign_to_move.cpp
        src/test/unit/unit_assignment_combinations.cpp
        src/test/unit/unit_assignments.cpp
        src/test/unit/unit_at.cpp
        src/test/unit/unit_calcMaxNumElementsAllowed.cpp
        src/test/unit/unit_calcsize.cpp
        src/test/unit/unit_compact.cpp
        src/test/unit/unit_copyassignment.cpp
        src/test/unit/unit_count.cpp
        src/test/unit/unit_diamond.cpp
        src/test/unit/unit_empty.cpp
        src/test/unit/unit_explicitctor.cpp
        src/test/unit/unit_fallback_hash.cpp
        src/test/unit/unit_hash_char_types.cpp
        src/test/unit/unit_hash_smart_ptr.cpp
        src/test/unit/unit_hash_string_view.cpp
        src/test/unit/unit_heterogeneous.cpp
        src/test/unit/unit_include_only.cpp
        src/test/unit/unit_initializer_list_insert.cpp
        src/test/unit/unit_initializerlist.cpp
        src/test/unit/unit_insert.cpp
        src/test/unit/unit_insert_collision.cpp
        src/test/unit/unit_insert_or_assign.cpp
        src/test/unit/unit_iterator_twice_bug.cpp
        src/test/unit/unit_iterators_ctor.cpp
        src/test/unit/unit_iterators_empty.cpp
        src/test/unit/unit_iterators_erase.cpp
        src/test/unit/unit_iterators_insert.cpp
        src/test/unit/unit_iterators_postinc.cpp
        src/test/unit/unit_iterators_stochastic.cpp
        src/test/unit/unit_load_factor.cpp
        src/test/unit/unit_maps_of_maps.cpp
        src/test/unit/unit_memleak_reserve.cpp
        src/test/unit/unit_multiple_apis.cpp
        src/test/unit/unit_mup.cpp
        src/test/unit/unit_no_intrinsics.cpp
        src/test/unit/unit_not_copyable.cpp
        src/test/unit/unit_not_moveable.cpp
        src/test/unit/unit_overflow.cpp
        src/test/unit/unit_overflow2.cpp
        src/test/unit/unit_overflow_collisions.cpp
        src/test/unit/unit_pair_operators.cpp
        src/test/unit/unit_pair_trivial.cpp
        src/test/unit/unit_playback.cpp
        src/test/unit/unit_random_verifier.cpp
        src/test/unit/unit_reserve.cpp
        src/test/unit/unit_reserve_and_assign.cpp
        src/test/unit/unit_rotr.cpp
        src/test/unit/unit_scoped_free.cpp
        src/test/unit/unit_sfc64_is_deterministic.cpp
        src/test/unit/unit_sizeof.cpp
        src/test/unit/unit_string.cpp
        src/test/unit/unit_try_emplace.cpp
        src/test/unit/unit_undefined_behavior_nekrolm.cpp
        src/test/unit/unit_unique_ptr.cpp
        src/test/unit/unit_unordered_set.cpp
        src/test/unit/unit_vectorofmaps.cpp
        src/test/unit/unit_xy.cpp)
