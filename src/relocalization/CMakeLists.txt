add_library(dsl_relocalization
feature_extractor.cc
sp_extractor.cc
feature_matcher.cc
sp_matcher.cc
vocabulary_binary.cc
struct/map_point.cc
struct/frame.cc
struct/virtual_frame.cc
struct/clique.cc
struct/vlad_database.cc
struct/key_frame_database.cc
struct/motion_estimator.cc
reloc_optimization/optimizer.cc
reloc_optimization/reprojection_functor.cc
reloc_optimization/surfel_reprojection_functor.cc
visualization/drawer.cc
relocalization_config.cc
pnp_solver.cc
converter.cc
desc_map_updater.cc
desc_map_optimizer.cc
desc_map_unused.cc
desc_map.cc
)

add_dependencies(
dsl_relocalization
dsl_util
DBoW2
)