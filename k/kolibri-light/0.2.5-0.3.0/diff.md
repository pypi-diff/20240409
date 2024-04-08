# Comparing `tmp/kolibri_light-0.2.5-py3-none-any.whl.zip` & `tmp/kolibri_light-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,707 +1,782 @@
-Zip file size: 1305576 bytes, number of entries: 705
--rw-r--r--  2.0 unx        5 b- defN 23-Aug-25 15:11 kolibri/VERSION
--rw-r--r--  2.0 unx     4359 b- defN 23-Aug-25 14:14 kolibri/__init__.py
--rw-r--r--  2.0 unx    16782 b- defN 23-Jul-09 11:29 kolibri/app.py
--rw-r--r--  2.0 unx     3190 b- defN 23-Jul-09 11:29 kolibri/config.py
--rw-r--r--  2.0 unx     1902 b- defN 23-Jul-09 11:29 kolibri/config_loader.py
--rw-r--r--  2.0 unx     3814 b- defN 23-Aug-11 17:50 kolibri/default_configs.py
--rw-r--r--  2.0 unx     5968 b- defN 23-Aug-11 18:09 kolibri/errors.py
--rw-r--r--  2.0 unx      795 b- defN 23-Jul-09 11:29 kolibri/logger.py
--rw-r--r--  2.0 unx     2219 b- defN 23-Jul-09 11:29 kolibri/metadata.py
--rw-r--r--  2.0 unx    10923 b- defN 23-Jul-09 11:29 kolibri/model_loader.py
--rw-r--r--  2.0 unx    25966 b- defN 23-Jul-09 11:29 kolibri/model_trainer.py
--rw-r--r--  2.0 unx     2763 b- defN 23-Jul-09 11:29 kolibri/registry.py
--rw-r--r--  2.0 unx      153 b- defN 23-Jul-09 11:29 kolibri/requirements.txt
--rw-r--r--  2.0 unx     2490 b- defN 23-Jul-09 11:29 kolibri/settings.py
--rw-r--r--  2.0 unx      457 b- defN 23-Jul-09 11:29 kolibri/settings.yaml
--rw-r--r--  2.0 unx      361 b- defN 23-Jul-09 11:29 kolibri/types.py
--rw-r--r--  2.0 unx      166 b- defN 23-Jul-09 11:29 kolibri/version.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 19:28 kolibri/api/__init__.py
--rw-r--r--  2.0 unx     2707 b- defN 23-Aug-21 19:28 kolibri/api/classification/__init__.py
--rw-r--r--  2.0 unx       66 b- defN 23-Jul-09 11:29 kolibri/autolearn/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/autolearn/metalearn/__init__.py
--rw-r--r--  2.0 unx     3125 b- defN 23-Jul-09 11:29 kolibri/autolearn/metalearn/metafeature.py
--rw-r--r--  2.0 unx    46866 b- defN 23-Jul-09 11:29 kolibri/autolearn/metalearn/metafeatures.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/autolearn/model_zoo/__init__.py
--rw-r--r--  2.0 unx     4737 b- defN 23-Aug-11 18:09 kolibri/autolearn/model_zoo/zoo_classifier.py
--rw-r--r--  2.0 unx     5834 b- defN 23-Aug-11 17:50 kolibri/autolearn/model_zoo/zoo_estimator.py
--rw-r--r--  2.0 unx     4246 b- defN 23-Jul-09 11:29 kolibri/autolearn/model_zoo/zoo_regressor.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/automl/__init__.py
--rw-r--r--  2.0 unx    15341 b- defN 23-Jul-09 11:29 kolibri/automl/data_inspection.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-25 14:14 kolibri/backend/__init__.py
--rw-r--r--  2.0 unx     6230 b- defN 23-Jul-09 11:29 kolibri/backend/models.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/backend/base/__init__.py
--rw-r--r--  2.0 unx    11844 b- defN 23-Aug-25 14:14 kolibri/backend/base/base_classifier.py
--rw-r--r--  2.0 unx     3916 b- defN 23-Jul-09 11:29 kolibri/backend/base/base_clustering.py
--rw-r--r--  2.0 unx    30797 b- defN 23-Aug-25 14:31 kolibri/backend/base/base_estimator.py
--rw-r--r--  2.0 unx     7418 b- defN 23-Aug-25 14:30 kolibri/backend/base/base_regressor.py
--rw-r--r--  2.0 unx    14321 b- defN 23-Jul-09 11:29 kolibri/backend/base/estimator.py
--rw-r--r--  2.0 unx      912 b- defN 23-Jul-09 11:29 kolibri/backend/base/nn_model.py
--rw-r--r--  2.0 unx      449 b- defN 23-Jul-09 11:29 kolibri/backend/bn/BayesianModel.py
--rw-r--r--  2.0 unx    44071 b- defN 23-Jul-09 11:29 kolibri/backend/bn/BayesianNetwork.py
--rw-r--r--  2.0 unx    24029 b- defN 23-Jul-09 11:29 kolibri/backend/bn/CPD.py
--rw-r--r--  2.0 unx     8931 b- defN 23-Jul-09 11:29 kolibri/backend/bn/ContinuousFactor.py
--rw-r--r--  2.0 unx    40531 b- defN 23-Jul-09 11:29 kolibri/backend/bn/DAG.py
--rw-r--r--  2.0 unx    28630 b- defN 23-Jul-09 11:29 kolibri/backend/bn/DiscreteFactor.py
--rw-r--r--  2.0 unx    31370 b- defN 23-Jul-09 11:29 kolibri/backend/bn/DynamicBayesianNetwork.py
--rw-r--r--  2.0 unx     4289 b- defN 23-Jul-09 11:29 kolibri/backend/bn/EliminationOrder.py
--rw-r--r--  2.0 unx    39930 b- defN 23-Jul-09 11:29 kolibri/backend/bn/ExactInference.py
--rw-r--r--  2.0 unx    10515 b- defN 23-Jul-09 11:29 kolibri/backend/bn/FactorGraph.py
--rw-r--r--  2.0 unx    14252 b- defN 23-Jul-09 11:29 kolibri/backend/bn/Independencies.py
--rw-r--r--  2.0 unx    11089 b- defN 23-Jul-09 11:29 kolibri/backend/bn/JointProbabilityDistribution.py
--rw-r--r--  2.0 unx     3058 b- defN 23-Jul-09 11:29 kolibri/backend/bn/JunctionTree.py
--rw-r--r--  2.0 unx     8219 b- defN 23-Jul-09 11:29 kolibri/backend/bn/LinearGaussianCPD.py
--rw-r--r--  2.0 unx    13783 b- defN 23-Jul-09 11:29 kolibri/backend/bn/MarkovChain.py
--rw-r--r--  2.0 unx    17804 b- defN 23-Jul-09 11:29 kolibri/backend/bn/MarkovNetwork.py
--rw-r--r--  2.0 unx     5791 b- defN 23-Jul-09 11:29 kolibri/backend/bn/NaiveBayes.py
--rw-r--r--  2.0 unx    24083 b- defN 23-Jul-09 11:29 kolibri/backend/bn/Sampling.py
--rw-r--r--  2.0 unx     9237 b- defN 23-Jul-09 11:29 kolibri/backend/bn/UndirectedGraph.py
--rw-r--r--  2.0 unx      723 b- defN 23-Jul-09 11:29 kolibri/backend/bn/__init__.py
--rw-r--r--  2.0 unx    11145 b- defN 23-Jul-09 11:29 kolibri/backend/bn/base_estimator.py
--rw-r--r--  2.0 unx     7604 b- defN 23-Jul-09 11:29 kolibri/backend/bn/base_inference.py
--rw-r--r--  2.0 unx    48040 b- defN 23-Aug-25 14:14 kolibri/backend/bn/bnlearn.py
--rw-r--r--  2.0 unx     3207 b- defN 23-Jul-09 11:29 kolibri/backend/bn/factors_base.py
--rw-r--r--  2.0 unx     2348 b- defN 23-Jul-09 11:29 kolibri/backend/bn/metrics.py
--rw-r--r--  2.0 unx    12326 b- defN 23-Aug-25 14:14 kolibri/backend/bn/network.py
--rw-r--r--  2.0 unx     3178 b- defN 23-Jul-09 11:29 kolibri/backend/bn/state_name.py
--rw-r--r--  2.0 unx    30222 b- defN 23-Jul-09 11:29 kolibri/backend/bn/tabulate.py
--rw-r--r--  2.0 unx     5326 b- defN 23-Jul-09 11:29 kolibri/backend/bn/utils.py
--rw-r--r--  2.0 unx    13476 b- defN 23-Jul-09 11:29 kolibri/backend/bn/distributions/CanonicalDistribution.py
--rw-r--r--  2.0 unx    11847 b- defN 23-Jul-09 11:29 kolibri/backend/bn/distributions/CustomDistribution.py
--rw-r--r--  2.0 unx    19195 b- defN 23-Jul-09 11:29 kolibri/backend/bn/distributions/GaussianDistribution.py
--rw-r--r--  2.0 unx      220 b- defN 23-Jul-09 11:29 kolibri/backend/bn/distributions/__init__.py
--rw-r--r--  2.0 unx      841 b- defN 23-Jul-09 11:29 kolibri/backend/bn/distributions/base.py
--rw-r--r--  2.0 unx    12715 b- defN 23-Jul-09 11:29 kolibri/backend/bn/estimators/HillClimbSearch.py
--rw-r--r--  2.0 unx     4805 b- defN 23-Jul-09 11:29 kolibri/backend/bn/estimators/MLE.py
--rw-r--r--  2.0 unx     4221 b- defN 23-Jul-09 11:29 kolibri/backend/bn/estimators/ScoreCache.py
--rw-r--r--  2.0 unx    18012 b- defN 23-Jul-09 11:29 kolibri/backend/bn/estimators/StructureScore.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/backend/bn/estimators/__init__.py
--rw-r--r--  2.0 unx     7985 b- defN 23-Jul-09 11:29 kolibri/backend/bn/estimators/bayesianEstimator.py
--rw-r--r--  2.0 unx       57 b- defN 23-Jul-09 11:29 kolibri/backend/bn/inference/__init__.py
--rw-r--r--  2.0 unx     3044 b- defN 23-Jul-09 11:29 kolibri/backend/bn/inference/inference.py
--rw-r--r--  2.0 unx      194 b- defN 23-Jul-09 11:29 kolibri/backend/bn/inference/predict.py
--rw-r--r--  2.0 unx      130 b- defN 23-Jul-09 11:29 kolibri/backend/bn/parameters/__init__.py
--rw-r--r--  2.0 unx      490 b- defN 23-Jul-09 11:29 kolibri/backend/bn/parameters/learn.py
--rw-r--r--  2.0 unx    12213 b- defN 23-Jul-09 11:29 kolibri/backend/bn/parameters/parameter_learning.py
--rw-r--r--  2.0 unx    18288 b- defN 23-Jul-09 11:29 kolibri/backend/bn/readwrite/BIF.py
--rw-r--r--  2.0 unx    14034 b- defN 23-Jul-09 11:29 kolibri/backend/bn/readwrite/UAI.py
--rw-r--r--  2.0 unx    16390 b- defN 23-Jul-09 11:29 kolibri/backend/bn/readwrite/XMLBIF.py
--rw-r--r--  2.0 unx      491 b- defN 23-Jul-09 11:29 kolibri/backend/bn/readwrite/__init__.py
--rw-r--r--  2.0 unx      311 b- defN 23-Jul-09 11:29 kolibri/backend/bn/structure/__init__.py
--rw-r--r--  2.0 unx     7020 b- defN 23-Jul-09 11:29 kolibri/backend/bn/structure/base.py
--rw-r--r--  2.0 unx     8354 b- defN 23-Jul-09 11:29 kolibri/backend/bn/structure/evaluation.py
--rw-r--r--  2.0 unx     1989 b- defN 23-Jul-09 11:29 kolibri/backend/bn/structure/learn.py
--rw-r--r--  2.0 unx     7267 b- defN 23-Jul-09 11:29 kolibri/backend/bn/structure/linear.py
--rw-r--r--  2.0 unx     7902 b- defN 23-Jul-09 11:29 kolibri/backend/bn/structure/low_rank.py
--rw-r--r--  2.0 unx    22607 b- defN 23-Jul-09 11:29 kolibri/backend/bn/structure/no_tears.py
--rw-r--r--  2.0 unx     2961 b- defN 23-Jul-09 11:29 kolibri/backend/bn/structure/no_tears_tf.py
--rw-r--r--  2.0 unx     1898 b- defN 23-Jul-09 11:29 kolibri/backend/bn/structure/no_tears_tf2.py
--rw-r--r--  2.0 unx     2961 b- defN 23-Jul-09 11:29 kolibri/backend/bn/structure/no_tears_tf_bak.py
--rw-r--r--  2.0 unx     8816 b- defN 23-Jul-09 11:29 kolibri/backend/bn/structure/nonlinear.py
--rw-r--r--  2.0 unx     4376 b- defN 23-Jul-09 11:29 kolibri/backend/bn/structure/notears_tf2.py
--rw-r--r--  2.0 unx     4208 b- defN 23-Jul-09 11:29 kolibri/backend/bn/structure/plot_dag.py
--rw-r--r--  2.0 unx    13671 b- defN 23-Jul-09 11:29 kolibri/backend/bn/structure/structure_model.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/backend/generators/__init__.py
--rw-r--r--  2.0 unx      157 b- defN 23-Aug-21 19:28 kolibri/backend/sklearn/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 19:28 kolibri/backend/sklearn/extensions/__init__.py
--rw-r--r--  2.0 unx    18744 b- defN 23-Aug-21 19:28 kolibri/backend/sklearn/extensions/decision_tree_log_reg.py
--rw-r--r--  2.0 unx     1100 b- defN 23-Aug-21 19:28 kolibri/backend/sklearn/extensions/distributed_nn.py
--rw-r--r--  2.0 unx    15651 b- defN 23-Aug-21 19:28 kolibri/backend/sklearn/extensions/lazy_learner.py
--rw-r--r--  2.0 unx    14741 b- defN 23-Aug-25 14:28 kolibri/backend/sklearn/extensions/lookup_learner.py
--rw-r--r--  2.0 unx       65 b- defN 23-Aug-21 19:28 kolibri/backend/sklearn/meta/__init__.py
--rw-r--r--  2.0 unx    13257 b- defN 23-Aug-21 19:28 kolibri/backend/sklearn/meta/chain_model.py
--rw-r--r--  2.0 unx    28317 b- defN 23-Aug-21 19:28 kolibri/backend/sklearn/meta/ecoc_model.py
--rw-r--r--  2.0 unx    28328 b- defN 23-Aug-21 19:28 kolibri/backend/sklearn/meta/ensemble_samplers.py
--rw-r--r--  2.0 unx     7646 b- defN 23-Aug-21 19:28 kolibri/backend/sklearn/meta/multi_output_estimator.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 19:28 kolibri/backend/sklearn/meta/ecoc/__init__.py
--rw-r--r--  2.0 unx     8616 b- defN 23-Aug-21 19:28 kolibri/backend/sklearn/meta/ecoc/code_matrix.py
--rw-r--r--  2.0 unx     5551 b- defN 23-Aug-21 19:28 kolibri/backend/sklearn/meta/ecoc/criterion.py
--rw-r--r--  2.0 unx     9095 b- defN 23-Aug-21 19:28 kolibri/backend/sklearn/meta/ecoc/decoder.py
--rw-r--r--  2.0 unx     3869 b- defN 23-Aug-21 19:28 kolibri/backend/sklearn/meta/ecoc/sffs.py
--rw-r--r--  2.0 unx     2953 b- defN 23-Aug-11 17:50 kolibri/backend/tensorflow/__init__.py
--rw-r--r--  2.0 unx      519 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/logger.py
--rw-r--r--  2.0 unx      308 b- defN 23-Aug-11 17:50 kolibri/backend/tensorflow/macros.py
--rw-r--r--  2.0 unx      457 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/autoencoder/__init__.py
--rw-r--r--  2.0 unx     7029 b- defN 23-Aug-25 14:14 kolibri/backend/tensorflow/autoencoder/base_autoencoder.py
--rw-r--r--  2.0 unx     3339 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/autoencoder/conv_autoencoder.py
--rw-r--r--  2.0 unx     2611 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/autoencoder/deep_autoencoder.py
--rw-r--r--  2.0 unx     3757 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/autoencoder/variational_autoencoder.py
--rw-r--r--  2.0 unx      204 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/autoencoder/decoders/__init__.py
--rw-r--r--  2.0 unx     2091 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/autoencoder/decoders/att_gru_decoder.py
--rw-r--r--  2.0 unx     1294 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/autoencoder/decoders/gru_decoder.py
--rw-r--r--  2.0 unx     1213 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/autoencoder/decoders/lstm_decoder.py
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/autoencoder/encoders/__init__.py
--rw-r--r--  2.0 unx     1257 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/autoencoder/encoders/gru_encoder.py
--rw-r--r--  2.0 unx     1383 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/autoencoder/encoders/lstm_encoder.py
--rw-r--r--  2.0 unx      134 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/callbacks/__init__.py
--rw-r--r--  2.0 unx     2025 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/callbacks/conll_call_back.py
--rw-r--r--  2.0 unx     2241 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/callbacks/eval_callBack.py
--rw-r--r--  2.0 unx     4874 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/callbacks/save_callback.py
--rw-r--r--  2.0 unx      320 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/embeddings/__init__.py
--rw-r--r--  2.0 unx     1709 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/embeddings/bare_embedding.py
--rw-r--r--  2.0 unx     4642 b- defN 23-Aug-25 14:14 kolibri/backend/tensorflow/embeddings/base_embedding.py
--rw-r--r--  2.0 unx     1322 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/embeddings/bert_embedding.py
--rw-r--r--  2.0 unx     8420 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/embeddings/elmo_embedding.py
--rw-r--r--  2.0 unx     3196 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/embeddings/embedding_trainer.py
--rw-r--r--  2.0 unx     1952 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/embeddings/fasttext_embedding.py
--rw-r--r--  2.0 unx     2568 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/embeddings/glove_embedding.py
--rw-r--r--  2.0 unx     9637 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/embeddings/loader.py
--rw-r--r--  2.0 unx    14296 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/embeddings/loader_albert.py
--rw-r--r--  2.0 unx     4114 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/embeddings/numeric_feature_embedding.py
--rw-r--r--  2.0 unx     4911 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/embeddings/stacked_embedding.py
--rw-r--r--  2.0 unx     3830 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/embeddings/transformer_embedding.py
--rw-r--r--  2.0 unx     3347 b- defN 23-Aug-25 14:14 kolibri/backend/tensorflow/embeddings/word_embedding.py
--rw-r--r--  2.0 unx      679 b- defN 23-Aug-11 17:50 kolibri/backend/tensorflow/gan/__init__.py
--rw-r--r--  2.0 unx    15332 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/gan/_transformer.py
--rw-r--r--  2.0 unx      462 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/gan/bgm.py
--rw-r--r--  2.0 unx     3406 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/gan/discriminator.py
--rw-r--r--  2.0 unx     2727 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/gan/generator.py
--rw-r--r--  2.0 unx      412 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/gan/ohe.py
--rw-r--r--  2.0 unx     1015 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/layers/__init__.py
--rw-r--r--  2.0 unx     3258 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/layers/att_wgt_avg_layer.py
--rw-r--r--  2.0 unx     1528 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/layers/behdanau_attention.py
--rw-r--r--  2.0 unx     4389 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/layers/conditional_random_field.py
--rw-r--r--  2.0 unx     1047 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/layers/folding_layer.py
--rw-r--r--  2.0 unx     4173 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/layers/gen_activation.py
--rw-r--r--  2.0 unx     2033 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/layers/highway_layer.py
--rw-r--r--  2.0 unx     3088 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/layers/kmax_pool_layer.py
--rw-r--r--  2.0 unx     1129 b- defN 23-Aug-11 17:50 kolibri/backend/tensorflow/layers/layer_utils.py
--rw-r--r--  2.0 unx     5012 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/layers/multi_head_attention.py
--rw-r--r--  2.0 unx      787 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/layers/non_masking_layer.py
--rw-r--r--  2.0 unx     1892 b- defN 23-Aug-11 17:50 kolibri/backend/tensorflow/layers/residual.py
--rw-r--r--  2.0 unx      372 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/losses/__init__.py
--rw-r--r--  2.0 unx     1416 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/losses/conditional_loss.py
--rw-r--r--  2.0 unx     2959 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/losses/custom_loses.py
--rw-r--r--  2.0 unx     2299 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/losses/gradient_penalty.py
--rw-r--r--  2.0 unx      292 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/metrics/__init__.py
--rw-r--r--  2.0 unx     2525 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/metrics/multi_label_classification.py
--rw-r--r--  2.0 unx    14331 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/metrics/sequence_labeling.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-25 14:14 kolibri/backend/tensorflow/tasks/__init__.py
--rw-r--r--  2.0 unx     5384 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/tasks/base_model.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/tasks/structured/__init__.py
--rw-r--r--  2.0 unx     7871 b- defN 23-Aug-15 22:12 kolibri/backend/tensorflow/tasks/structured/base_model.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/tasks/structured/regression/__init__.py
--rw-r--r--  2.0 unx     4756 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/tasks/structured/regression/base_model.py
--rw-r--r--  2.0 unx     1802 b- defN 23-Aug-11 17:50 kolibri/backend/tensorflow/tasks/structured/regression/dnn_regression_estimator.py
--rw-r--r--  2.0 unx     2744 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/tasks/structured/regression/models.py
--rw-r--r--  2.0 unx      517 b- defN 23-Aug-11 17:50 kolibri/backend/tensorflow/tasks/structured/synthetic/__init__.py
--rw-r--r--  2.0 unx    20393 b- defN 23-Aug-11 17:50 kolibri/backend/tensorflow/tasks/structured/synthetic/_synthesizer.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 19:28 kolibri/backend/tensorflow/tasks/text/__init__.py
--rw-r--r--  2.0 unx      417 b- defN 23-Aug-21 19:28 kolibri/backend/tensorflow/tasks/text/classification/__init__.py
--rw-r--r--  2.0 unx    15208 b- defN 23-Aug-21 19:28 kolibri/backend/tensorflow/tasks/text/classification/base_model.py
--rw-r--r--  2.0 unx     3381 b- defN 23-Aug-21 19:28 kolibri/backend/tensorflow/tasks/text/classification/cnn_attention_model.py
--rw-r--r--  2.0 unx     6196 b- defN 23-Aug-21 19:28 kolibri/backend/tensorflow/tasks/text/classification/dpcnn_model.py
--rw-r--r--  2.0 unx    28815 b- defN 23-Aug-21 19:28 kolibri/backend/tensorflow/tasks/text/classification/models.py
--rw-r--r--  2.0 unx      429 b- defN 23-Aug-21 19:28 kolibri/backend/tensorflow/tasks/text/labeling/__init__.py
--rw-r--r--  2.0 unx    17329 b- defN 23-Aug-21 19:28 kolibri/backend/tensorflow/tasks/text/labeling/base_model.py
--rw-r--r--  2.0 unx     2846 b- defN 23-Aug-21 19:28 kolibri/backend/tensorflow/tasks/text/labeling/bi_gru_crf_model.py
--rw-r--r--  2.0 unx     2249 b- defN 23-Aug-21 19:28 kolibri/backend/tensorflow/tasks/text/labeling/bi_gru_model.py
--rw-r--r--  2.0 unx     2991 b- defN 23-Aug-21 19:28 kolibri/backend/tensorflow/tasks/text/labeling/bi_lstm_crf_model.py
--rw-r--r--  2.0 unx     2295 b- defN 23-Aug-21 19:28 kolibri/backend/tensorflow/tasks/text/labeling/bi_lstm_model.py
--rw-r--r--  2.0 unx     1440 b- defN 23-Aug-21 19:28 kolibri/backend/tensorflow/tasks/text/labeling/cnn_lstm_model.py
--rw-r--r--  2.0 unx       84 b- defN 23-Aug-21 19:28 kolibri/backend/tensorflow/tasks/text/seq2seq/__init__.py
--rw-r--r--  2.0 unx     2443 b- defN 23-Aug-21 19:28 kolibri/backend/tensorflow/tasks/text/seq2seq/generator.py
--rw-r--r--  2.0 unx    13913 b- defN 23-Aug-21 19:28 kolibri/backend/tensorflow/tasks/text/seq2seq/model.py
--rw-r--r--  2.0 unx     1203 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/utils/__init__.py
--rw-r--r--  2.0 unx      740 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/utils/_load_demo.py
--rw-r--r--  2.0 unx      919 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/utils/data.py
--rw-r--r--  2.0 unx     1629 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/utils/model.py
--rw-r--r--  2.0 unx     1131 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/utils/multi_label.py
--rw-r--r--  2.0 unx      862 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/utils/serialize.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 19:28 kolibri/backend/torch/__init__.py
--rw-r--r--  2.0 unx    12666 b- defN 23-Aug-21 19:28 kolibri/backend/torch/base_model.py
--rw-r--r--  2.0 unx     8161 b- defN 23-Aug-21 19:28 kolibri/backend/torch/models.py
--rw-r--r--  2.0 unx      305 b- defN 23-Aug-21 19:28 kolibri/backend/torch/utils.py
--rw-r--r--  2.0 unx      671 b- defN 23-Aug-21 19:28 kolibri/backend/torch/golem_utils/__init__.py
--rw-r--r--  2.0 unx     4438 b- defN 23-Aug-21 19:28 kolibri/backend/torch/golem_utils/golem_model.py
--rw-r--r--  2.0 unx     2545 b- defN 23-Aug-21 19:28 kolibri/backend/torch/golem_utils/train.py
--rw-r--r--  2.0 unx     1636 b- defN 23-Aug-21 19:28 kolibri/backend/torch/golem_utils/utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 19:28 kolibri/backend/torch/layers/__init__.py
--rw-r--r--  2.0 unx     5973 b- defN 23-Aug-21 19:28 kolibri/backend/torch/layers/crf.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 19:28 kolibri/backend/torch/tasks/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 19:28 kolibri/backend/torch/tasks/text/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 19:28 kolibri/backend/torch/tasks/text/labeling/__init__.py
--rw-r--r--  2.0 unx     1836 b- defN 23-Aug-21 19:28 kolibri/backend/torch/tasks/text/labeling/bi_lstm_crf.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 19:28 kolibri/backend/torch/utils/__init__.py
--rw-r--r--  2.0 unx     4009 b- defN 23-Aug-21 19:28 kolibri/backend/torch/utils/lbfgsb_scipy.py
--rw-r--r--  2.0 unx     2864 b- defN 23-Aug-21 19:28 kolibri/backend/torch/utils/locally_connected.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 19:28 kolibri/bin/__init__.py
--rw-r--r--  2.0 unx      471 b- defN 23-Aug-21 19:28 kolibri/bin/datasets_configs.json
--rw-r--r--  2.0 unx     2731 b- defN 23-Aug-21 19:28 kolibri/bin/kolibri-download.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-25 14:14 kolibri/callbacks/__init__.py
--rw-r--r--  2.0 unx      536 b- defN 23-Aug-25 14:14 kolibri/callbacks/base.py
--rw-r--r--  2.0 unx     3298 b- defN 23-Aug-25 14:14 kolibri/callbacks/callbacks_manager.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/core/__init__.py
--rw-r--r--  2.0 unx    18812 b- defN 23-Aug-11 17:50 kolibri/core/component.py
--rw-r--r--  2.0 unx      223 b- defN 23-Aug-11 18:09 kolibri/core/document.py
--rw-r--r--  2.0 unx     1111 b- defN 23-Jul-09 11:29 kolibri/core/entity.py
--rw-r--r--  2.0 unx     4052 b- defN 23-Jul-09 11:29 kolibri/core/modules.py
--rw-r--r--  2.0 unx    17570 b- defN 23-Jul-09 11:29 kolibri/core/pipeline.py
--rw-r--r--  2.0 unx     2289 b- defN 23-Jul-09 11:29 kolibri/core/serializable.py
--rw-r--r--  2.0 unx     5771 b- defN 23-Jul-09 11:29 kolibri/core/vocabulary.py
--rw-r--r--  2.0 unx      117 b- defN 23-Aug-25 14:14 kolibri/data/__init__.py
--rw-r--r--  2.0 unx     4452 b- defN 23-Jun-18 21:58 kolibri/data/auto_downloader.py
--rw-r--r--  2.0 unx     2246 b- defN 23-Jun-18 21:58 kolibri/data/base_stream.py
--rw-r--r--  2.0 unx     4978 b- defN 23-Aug-25 14:14 kolibri/data/blob.py
--rw-r--r--  2.0 unx    29540 b- defN 23-Jun-18 21:58 kolibri/data/dataset.py
--rw-r--r--  2.0 unx      234 b- defN 23-Jul-08 17:41 kolibri/data/document.py
--rw-r--r--  2.0 unx    39086 b- defN 23-Jun-18 21:58 kolibri/data/downloader.py
--rw-r--r--  2.0 unx    10372 b- defN 23-Jun-18 21:58 kolibri/data/file_stream.py
--rw-r--r--  2.0 unx      534 b- defN 23-Jun-18 21:58 kolibri/data/iterator.py
--rw-r--r--  2.0 unx      743 b- defN 23-Jun-18 21:58 kolibri/data/resources.py
--rw-r--r--  2.0 unx    10130 b- defN 23-Jun-18 21:58 kolibri/data/schemes.py
--rw-r--r--  2.0 unx    42659 b- defN 23-May-21 07:09 kolibri/data/settings.py
--rw-r--r--  2.0 unx     5610 b- defN 23-Jun-18 21:58 kolibri/data/streams.py
--rw-r--r--  2.0 unx     7910 b- defN 23-Jun-18 21:58 kolibri/data/text.py
--rw-r--r--  2.0 unx    43985 b- defN 23-Aug-25 14:14 kolibri/data/utils.py
--rw-r--r--  2.0 unx       94 b- defN 23-Jun-18 21:58 kolibri/data/format/__init__.py
--rw-r--r--  2.0 unx      539 b- defN 23-Jun-18 21:58 kolibri/data/format/conll.py
--rw-r--r--  2.0 unx      385 b- defN 23-Jun-18 21:58 kolibri/data/format/csv.py
--rw-r--r--  2.0 unx      149 b- defN 23-Aug-25 14:14 kolibri/data/loaders/__init__.py
--rw-r--r--  2.0 unx      960 b- defN 23-Jul-08 17:41 kolibri/data/loaders/arxiv.py
--rw-r--r--  2.0 unx     2516 b- defN 23-Jul-08 17:41 kolibri/data/loaders/base.py
--rw-r--r--  2.0 unx     2238 b- defN 23-Jul-08 17:41 kolibri/data/loaders/csv_loader.py
--rw-r--r--  2.0 unx     4578 b- defN 23-Aug-25 14:14 kolibri/data/loaders/pdf.py
--rw-r--r--  2.0 unx     1973 b- defN 23-Jul-08 17:41 kolibri/data/loaders/text.py
--rw-r--r--  2.0 unx     7710 b- defN 23-Jul-08 17:41 kolibri/data/loaders/web_base.py
--rw-r--r--  2.0 unx      242 b- defN 23-Jul-08 17:41 kolibri/data/parsers/__init__.py
--rw-r--r--  2.0 unx     1929 b- defN 23-Jul-08 17:41 kolibri/data/parsers/audio.py
--rw-r--r--  2.0 unx     1090 b- defN 23-Jul-08 17:41 kolibri/data/parsers/base.py
--rw-r--r--  2.0 unx     2429 b- defN 23-Jul-08 17:41 kolibri/data/parsers/generic.py
--rw-r--r--  2.0 unx      813 b- defN 23-Jul-08 17:41 kolibri/data/parsers/pdf.py
--rw-r--r--  2.0 unx      906 b- defN 23-Jul-08 17:41 kolibri/data/parsers/registry.py
--rw-r--r--  2.0 unx      453 b- defN 23-Jul-08 17:41 kolibri/data/parsers/txt.py
--rw-r--r--  2.0 unx       85 b- defN 23-Jul-08 17:41 kolibri/data/parsers/html/__init__.py
--rw-r--r--  2.0 unx     1567 b- defN 23-Jul-08 17:41 kolibri/data/parsers/html/bs4.py
--rw-r--r--  2.0 unx      929 b- defN 23-Jul-08 17:41 kolibri/data/parsers/html/hyperlinks.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-21 07:09 kolibri/data/text/__init__.py
--rw-r--r--  2.0 unx     2246 b- defN 23-Jun-06 21:58 kolibri/data/text/base_stream.py
--rw-r--r--  2.0 unx     1236 b- defN 23-Jun-18 21:58 kolibri/data/text/corpus.py
--rw-r--r--  2.0 unx    29550 b- defN 23-May-21 07:09 kolibri/data/text/dataset.py
--rw-r--r--  2.0 unx    10385 b- defN 23-Jun-06 21:58 kolibri/data/text/file_stream.py
--rw-r--r--  2.0 unx     5145 b- defN 23-Jun-18 21:58 kolibri/data/text/generators.py
--rw-r--r--  2.0 unx      534 b- defN 23-May-21 07:09 kolibri/data/text/iterator.py
--rw-r--r--  2.0 unx    10130 b- defN 23-May-21 07:09 kolibri/data/text/schemes.py
--rw-r--r--  2.0 unx     5615 b- defN 23-May-21 07:09 kolibri/data/text/streams.py
--rw-r--r--  2.0 unx     7915 b- defN 23-May-21 07:09 kolibri/data/text/text.py
--rw-r--r--  2.0 unx      104 b- defN 23-Jun-06 21:58 kolibri/data/text/format/__init__.py
--rw-r--r--  2.0 unx      539 b- defN 23-Jun-06 21:58 kolibri/data/text/format/conll.py
--rw-r--r--  2.0 unx      385 b- defN 23-Jun-06 21:58 kolibri/data/text/format/csv.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-21 07:09 kolibri/data/text/quality/__init__.py
--rw-r--r--  2.0 unx     4796 b- defN 23-Jun-18 21:58 kolibri/data/text/quality/cosineSimilarity.py
--rw-r--r--  2.0 unx      983 b- defN 23-May-21 07:09 kolibri/data/text/quality/mismatch.py
--rw-r--r--  2.0 unx      166 b- defN 23-Jun-18 21:58 kolibri/data/text/quality/pairwise_cos_sim.py
--rw-r--r--  2.0 unx      837 b- defN 23-Jun-18 21:58 kolibri/data/text/quality/similar.py
--rw-r--r--  2.0 unx       47 b- defN 23-Aug-21 19:28 kolibri/datasets/__init__.py
--rw-r--r--  2.0 unx     1800 b- defN 23-Aug-21 19:28 kolibri/datasets/read_data.py
--rw-r--r--  2.0 unx       61 b- defN 23-Aug-21 19:28 kolibri/datasets/reader/__init__.py
--rw-r--r--  2.0 unx     3092 b- defN 23-Aug-21 19:28 kolibri/datasets/reader/base_reader.py
--rw-r--r--  2.0 unx     4055 b- defN 23-Aug-21 19:28 kolibri/datasets/reader/classification.py
--rw-r--r--  2.0 unx     2213 b- defN 23-Aug-21 19:28 kolibri/datasets/reader/conll.py
--rw-r--r--  2.0 unx    30779 b- defN 23-Aug-21 19:28 kolibri/datasets/reader/dialogs_reader.py
--rw-r--r--  2.0 unx     8005 b- defN 23-Aug-21 19:28 kolibri/datasets/reader/dstc2.py
--rw-r--r--  2.0 unx     4919 b- defN 23-Aug-21 19:28 kolibri/datasets/reader/snips.py
--rw-r--r--  2.0 unx     3531 b- defN 23-Aug-25 14:06 kolibri/distances/__init__.py
--rw-r--r--  2.0 unx     4899 b- defN 23-Aug-25 14:06 kolibri/distances/base_categorical.py
--rw-r--r--  2.0 unx     2551 b- defN 23-Aug-25 14:06 kolibri/distances/eskin.py
--rw-r--r--  2.0 unx     3907 b- defN 23-Aug-25 14:06 kolibri/distances/goodall.py
--rw-r--r--  2.0 unx     6368 b- defN 23-Aug-25 14:06 kolibri/distances/heom.py
--rw-r--r--  2.0 unx     5015 b- defN 23-Aug-25 14:06 kolibri/distances/hvdm.py
--rw-r--r--  2.0 unx     1226 b- defN 23-Aug-25 14:06 kolibri/distances/lin.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/evaluation/__init__.py
--rw-r--r--  2.0 unx     7911 b- defN 23-Aug-25 14:14 kolibri/evaluation/classifier_evaluator.py
--rw-r--r--  2.0 unx     2489 b- defN 23-Jul-09 11:29 kolibri/evaluation/clustering_evaluator.py
--rw-r--r--  2.0 unx    41666 b- defN 23-Jul-09 11:29 kolibri/evaluation/model_plot.py
--rw-r--r--  2.0 unx      809 b- defN 23-Jul-09 11:29 kolibri/evaluation/metrics/__init__.py
--rw-r--r--  2.0 unx     5578 b- defN 23-Jul-09 11:29 kolibri/evaluation/metrics/anomaly.py
--rw-r--r--  2.0 unx     1792 b- defN 23-Jul-09 11:29 kolibri/evaluation/metrics/base_metric.py
--rw-r--r--  2.0 unx     9438 b- defN 23-Jul-09 11:29 kolibri/evaluation/metrics/classification.py
--rw-r--r--  2.0 unx     7198 b- defN 23-Jul-09 11:29 kolibri/evaluation/metrics/clustering.py
--rw-r--r--  2.0 unx     8757 b- defN 23-Jul-09 11:29 kolibri/evaluation/metrics/metric_utils.py
--rw-r--r--  2.0 unx     9491 b- defN 23-Jul-09 11:29 kolibri/evaluation/metrics/regression.py
--rw-r--r--  2.0 unx    10235 b- defN 23-Jul-09 11:29 kolibri/evaluation/metrics/time_series.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/evaluators/__init__.py
--rw-r--r--  2.0 unx     8796 b- defN 23-Jul-09 11:29 kolibri/evaluators/classifier_evaluator.py
--rw-r--r--  2.0 unx     2489 b- defN 23-Jul-09 11:29 kolibri/evaluators/clustering_evaluator.py
--rw-r--r--  2.0 unx    41682 b- defN 23-Jul-09 11:29 kolibri/evaluators/model_plot.py
--rw-r--r--  2.0 unx     3215 b- defN 23-Jul-28 21:31 kolibri/evaluators/synthetic_data.py
--rw-r--r--  2.0 unx      224 b- defN 23-Jul-09 11:29 kolibri/experiment_tracking/__init__.py
--rw-r--r--  2.0 unx     6170 b- defN 23-Jul-09 11:29 kolibri/experiment_tracking/experiment_logger.py
--rw-r--r--  2.0 unx     4971 b- defN 23-Jul-09 11:29 kolibri/experiment_tracking/mlflow_logger.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 19:28 kolibri/explainers/__init__.py
--rw-r--r--  2.0 unx    12089 b- defN 23-Aug-21 19:28 kolibri/explainers/shap_explainer.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-25 14:14 kolibri/features/__init__.py
--rw-r--r--  2.0 unx     2781 b- defN 23-Jul-09 11:29 kolibri/features/base_feature.py
--rw-r--r--  2.0 unx     1431 b- defN 23-Jul-09 11:29 kolibri/features/basefeaturizer.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/features/tabular/__init__.py
--rw-r--r--  2.0 unx     1763 b- defN 23-Jul-09 11:29 kolibri/features/tabular/time_serie_featurizer.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 19:28 kolibri/features/text/__init__.py
--rw-r--r--  2.0 unx     8352 b- defN 23-Aug-21 19:28 kolibri/features/text/feature_functions.py
--rw-r--r--  2.0 unx    10000 b- defN 23-Aug-21 19:28 kolibri/features/text/hashing_tfidf_vectorizer.py
--rw-r--r--  2.0 unx     5801 b- defN 23-Aug-21 19:28 kolibri/features/text/text_features.py
--rw-r--r--  2.0 unx     6336 b- defN 23-Aug-21 19:28 kolibri/features/text/tf_idf_featurizer.py
--rw-r--r--  2.0 unx     5853 b- defN 23-Aug-21 19:28 kolibri/features/text/tf_idf_topics_vectorizer.py
--rw-r--r--  2.0 unx     8121 b- defN 23-Aug-21 19:28 kolibri/features/text/tfidf_weighted_embedder.py
--rw-r--r--  2.0 unx      346 b- defN 23-Aug-21 19:28 kolibri/features/text/embedders/__init__.py
--rw-r--r--  2.0 unx     3709 b- defN 23-Aug-21 19:28 kolibri/features/text/embedders/base.py
--rw-r--r--  2.0 unx     1347 b- defN 23-Aug-21 19:28 kolibri/features/text/embedders/bow_embedder.py
--rw-r--r--  2.0 unx     9928 b- defN 23-Aug-21 19:28 kolibri/features/text/embedders/elmo_embedder.py
--rw-r--r--  2.0 unx     1568 b- defN 23-Aug-21 19:28 kolibri/features/text/embedders/fasttext_embedder.py
--rw-r--r--  2.0 unx     2027 b- defN 23-Aug-21 19:28 kolibri/features/text/embedders/glove_embedder.py
--rw-r--r--  2.0 unx     4096 b- defN 23-Aug-21 19:28 kolibri/features/text/embedders/llamacpp.py
--rw-r--r--  2.0 unx    17705 b- defN 23-Aug-21 19:28 kolibri/features/text/embedders/openai.py
--rw-r--r--  2.0 unx     2466 b- defN 23-Aug-21 19:28 kolibri/features/text/embedders/tensorflow_hub.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/features/timeseries/__init__.py
--rw-r--r--  2.0 unx    31971 b- defN 23-Jul-09 11:29 kolibri/features/timeseries/features_utils.py
--rw-r--r--  2.0 unx    10656 b- defN 23-Jul-09 11:29 kolibri/features/timeseries/ts_featurizer.py
--rw-r--r--  2.0 unx     7659 b- defN 23-Jul-09 11:29 kolibri/features/timeseries/utils.py
--rw-r--r--  2.0 unx      358 b- defN 23-Jul-09 11:29 kolibri/features/timeseries/feature_extraction/__init__.py
--rw-r--r--  2.0 unx    16661 b- defN 23-Jul-09 11:29 kolibri/features/timeseries/feature_extraction/data.py
--rw-r--r--  2.0 unx    13772 b- defN 23-Jul-09 11:29 kolibri/features/timeseries/feature_extraction/extraction.py
--rw-r--r--  2.0 unx    81555 b- defN 23-Jul-09 11:29 kolibri/features/timeseries/feature_extraction/feature_calculators.py
--rw-r--r--  2.0 unx    14105 b- defN 23-Jul-09 11:29 kolibri/features/timeseries/feature_extraction/settings.py
--rw-r--r--  2.0 unx      606 b- defN 23-Jul-09 11:29 kolibri/features/timeseries/feature_selection/__init__.py
--rw-r--r--  2.0 unx    15671 b- defN 23-Jul-09 11:29 kolibri/features/timeseries/feature_selection/relevance.py
--rw-r--r--  2.0 unx     7871 b- defN 23-Jul-09 11:29 kolibri/features/timeseries/feature_selection/selection.py
--rw-r--r--  2.0 unx     8691 b- defN 23-Jul-09 11:29 kolibri/features/timeseries/feature_selection/significance_tests.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 19:28 kolibri/formers/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 19:28 kolibri/formers/tabular/__init__.py
--rw-r--r--  2.0 unx     1043 b- defN 23-Aug-21 19:28 kolibri/formers/tabular/clustering.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 19:28 kolibri/formers/text/__init__.py
--rw-r--r--  2.0 unx     4315 b- defN 23-Aug-21 19:28 kolibri/formers/text/classifier.py
--rw-r--r--  2.0 unx      230 b- defN 23-Aug-21 19:28 kolibri/formers/text/sentiment.py
--rw-r--r--  2.0 unx     4515 b- defN 23-Aug-21 19:28 kolibri/formers/text/similarity.py
--rw-r--r--  2.0 unx    40754 b- defN 23-Aug-21 19:28 kolibri/formers/text/topic_former.py
--rw-r--r--  2.0 unx        1 b- defN 23-Aug-25 14:14 kolibri/indexers/__init__.py
--rw-r--r--  2.0 unx     2657 b- defN 23-Aug-25 14:14 kolibri/indexers/base_indexer.py
--rw-r--r--  2.0 unx     1239 b- defN 23-Jul-09 11:29 kolibri/indexers/kolibri_label_encoder.py
--rw-r--r--  2.0 unx     3490 b- defN 23-Aug-25 14:14 kolibri/indexers/label_indexer.py
--rw-r--r--  2.0 unx     1248 b- defN 23-Jul-09 11:29 kolibri/indexers/multi_content_indexer.py
--rw-r--r--  2.0 unx     2394 b- defN 23-Jul-09 11:29 kolibri/indexers/multi_target_indexer.py
--rw-r--r--  2.0 unx     4944 b- defN 23-Jul-09 11:29 kolibri/indexers/sequence_char_indexer.py
--rw-r--r--  2.0 unx     6012 b- defN 23-Jul-25 15:43 kolibri/indexers/sequence_indexer.py
--rw-r--r--  2.0 unx     5940 b- defN 23-Jul-09 11:29 kolibri/indexers/text_indexer.py
--rw-r--r--  2.0 unx       43 b- defN 23-Jul-09 11:29 kolibri/knowledge/__init__.py
--rw-r--r--  2.0 unx     1173 b- defN 23-Jul-09 11:29 kolibri/knowledge/domain.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-25 14:14 kolibri/llms/__init__.py
--rw-r--r--  2.0 unx     5183 b- defN 23-Aug-25 14:14 kolibri/llms/base.py
--rw-r--r--  2.0 unx    25099 b- defN 23-Aug-25 14:14 kolibri/llms/openai.py
--rw-r--r--  2.0 unx    11163 b- defN 23-Jul-09 11:29 kolibri/mlflow/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/optimizers/__init__.py
--rw-r--r--  2.0 unx     9226 b- defN 23-Jul-09 11:29 kolibri/optimizers/metric.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/optimizers/optuna/__init__.py
--rw-r--r--  2.0 unx    10868 b- defN 23-Jul-09 11:29 kolibri/optimizers/optuna/objective.py
--rw-r--r--  2.0 unx     2889 b- defN 23-Jul-09 11:29 kolibri/optimizers/optuna/tuner.py
--rw-r--r--  2.0 unx       49 b- defN 23-Aug-21 19:28 kolibri/output/__init__.py
--rw-r--r--  2.0 unx     3303 b- defN 23-Aug-21 19:28 kolibri/output/display.py
--rw-r--r--  2.0 unx     5694 b- defN 23-Aug-21 19:28 kolibri/output/display_backend.py
--rw-r--r--  2.0 unx     1637 b- defN 23-Aug-21 19:28 kolibri/output/display_component.py
--rw-r--r--  2.0 unx     4514 b- defN 23-Aug-21 19:28 kolibri/output/progress_bar.py
--rw-r--r--  2.0 unx       40 b- defN 23-Jul-09 11:29 kolibri/preprocess/__init__.py
--rw-r--r--  2.0 unx    13211 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/DataFrameVectorizer.py
--rw-r--r--  2.0 unx     1780 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/__init__.py
--rw-r--r--  2.0 unx     3030 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/binning.py
--rw-r--r--  2.0 unx     8728 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/boruta_py.py
--rw-r--r--  2.0 unx     1837 b- defN 23-Aug-25 14:14 kolibri/preprocess/tabular/category_transformer.py
--rw-r--r--  2.0 unx     5219 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/cluster.py
--rw-r--r--  2.0 unx      783 b- defN 23-Aug-25 12:31 kolibri/preprocess/tabular/columns_remover.py
--rw-r--r--  2.0 unx     1556 b- defN 23-Aug-25 12:31 kolibri/preprocess/tabular/columns_transfromer.py
--rw-r--r--  2.0 unx    11658 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/data_imputer.py
--rw-r--r--  2.0 unx     2970 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/dummy_converter.py
--rw-r--r--  2.0 unx    13500 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/feature_interaction.py
--rw-r--r--  2.0 unx    10314 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/feature_selection.py
--rw-r--r--  2.0 unx     4401 b- defN 23-Aug-25 12:31 kolibri/preprocess/tabular/infer_datatype.py
--rw-r--r--  2.0 unx    13584 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/multicollinearity.py
--rw-r--r--  2.0 unx     4341 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/normalize.py
--rw-r--r--  2.0 unx     2494 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/one_hot_encoder_multi.py
--rw-r--r--  2.0 unx     1620 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/ordinal_transformer.py
--rw-r--r--  2.0 unx     2616 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/outlier_remover.py
--rw-r--r--  2.0 unx   149882 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/preprocess.py
--rw-r--r--  2.0 unx    20056 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/preprocessing_pipeline.py
--rw-r--r--  2.0 unx     3454 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/rare_levels.py
--rw-r--r--  2.0 unx     8598 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/reduce_cardinality.py
--rw-r--r--  2.0 unx     4848 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/reduce_dimensionality.py
--rw-r--r--  2.0 unx     1801 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/regression_target_transformer.py
--rw-r--r--  2.0 unx     2003 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/similar_features.py
--rw-r--r--  2.0 unx     4003 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/time_features_extractor.py
--rw-r--r--  2.0 unx     1808 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/univar_outliers.py
--rw-r--r--  2.0 unx     3531 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/zero_variance_remover.py
--rw-r--r--  2.0 unx       76 b- defN 23-Aug-21 19:28 kolibri/preprocess/text/__init__.py
--rw-r--r--  2.0 unx     4058 b- defN 23-Aug-21 19:28 kolibri/preprocess/text/capitalization.py
--rw-r--r--  2.0 unx      596 b- defN 23-Aug-21 19:28 kolibri/preprocess/text/char_splitter.py
--rw-r--r--  2.0 unx     4297 b- defN 23-Aug-21 19:28 kolibri/preprocess/text/collocation_analyzer.py
--rw-r--r--  2.0 unx     1412 b- defN 23-Aug-21 19:28 kolibri/preprocess/text/context_builder.py
--rw-r--r--  2.0 unx     3356 b- defN 23-Aug-21 19:28 kolibri/preprocess/text/dirty_comments_preprocessor.py
--rw-r--r--  2.0 unx     5305 b- defN 23-Aug-21 19:28 kolibri/preprocess/text/doc_chuncker.py
--rw-r--r--  2.0 unx     1183 b- defN 23-Aug-21 19:28 kolibri/preprocess/text/mask.py
--rw-r--r--  2.0 unx     7307 b- defN 23-Aug-21 19:28 kolibri/preprocess/text/ner_preprocessor.py
--rw-r--r--  2.0 unx     1229 b- defN 23-Aug-21 19:28 kolibri/preprocess/text/random_embeddings_matrix.py
--rw-r--r--  2.0 unx    10274 b- defN 23-Aug-21 19:28 kolibri/preprocess/text/re_preprocessor.py
--rw-r--r--  2.0 unx     5800 b- defN 23-Aug-21 19:28 kolibri/preprocess/text/siamese_preprocessor.py
--rw-r--r--  2.0 unx     1883 b- defN 23-Aug-21 19:28 kolibri/preprocess/text/str_token_reverser.py
--rw-r--r--  2.0 unx     7566 b- defN 23-Aug-21 19:28 kolibri/preprocess/text/str_utf8_encoder.py
--rw-r--r--  2.0 unx     6299 b- defN 23-Aug-21 19:28 kolibri/preprocess/text/text_splitter.py
--rw-r--r--  2.0 unx     2657 b- defN 23-Aug-21 19:28 kolibri/preprocess/text/transformers_preprocessor.py
--rw-r--r--  2.0 unx     5288 b- defN 23-Aug-21 19:28 kolibri/preprocess/text/cleaning/__email_configs.py
--rw-r--r--  2.0 unx       67 b- defN 23-Aug-21 19:28 kolibri/preprocess/text/cleaning/__init__.py
--rw-r--r--  2.0 unx     4348 b- defN 23-Aug-21 19:28 kolibri/preprocess/text/cleaning/cleaning_scripts.py
--rw-r--r--  2.0 unx    23554 b- defN 23-Aug-21 19:28 kolibri/preprocess/text/cleaning/email2text.py
--rw-r--r--  2.0 unx     1764 b- defN 23-Aug-21 19:28 kolibri/preprocess/text/cleaning/email_cleaner.py
--rw-r--r--  2.0 unx     1425 b- defN 23-Aug-21 19:28 kolibri/preprocess/text/cleaning/email_parser.py
--rw-r--r--  2.0 unx     3279 b- defN 23-Aug-21 19:28 kolibri/preprocess/text/cleaning/header_parser.py
--rw-r--r--  2.0 unx       82 b- defN 23-Aug-21 19:28 kolibri/preprocess/text/language_detection/__init__.py
--rw-r--r--  2.0 unx     1420 b- defN 23-Aug-21 19:28 kolibri/preprocess/text/language_detection/lang_detect.py
--rw-r--r--  2.0 unx     7047 b- defN 23-Aug-21 19:28 kolibri/preprocess/text/translation/Translate_.py
--rw-r--r--  2.0 unx     1079 b- defN 23-Aug-21 19:28 kolibri/preprocess/text/translation/__init__.py
--rw-r--r--  2.0 unx     9890 b- defN 23-Aug-21 19:28 kolibri/preprocess/text/translation/client.py
--rw-r--r--  2.0 unx     9746 b- defN 23-Aug-21 19:28 kolibri/preprocess/text/translation/constants.py
--rw-r--r--  2.0 unx     1601 b- defN 23-Aug-21 19:28 kolibri/preprocess/text/translation/models.py
--rw-r--r--  2.0 unx     6090 b- defN 23-Aug-21 19:28 kolibri/preprocess/text/translation/translate.py
--rw-r--r--  2.0 unx     2640 b- defN 23-Aug-21 19:28 kolibri/preprocess/text/translation/utils.py
--rw-r--r--  2.0 unx       65 b- defN 23-Jul-09 11:29 kolibri/preprocess/timeseries/__init__.py
--rw-r--r--  2.0 unx    16072 b- defN 23-Jul-09 11:29 kolibri/preprocess/timeseries/multi_window_generator.py
--rw-r--r--  2.0 unx    15304 b- defN 23-Jul-09 11:29 kolibri/preprocess/timeseries/multi_window_generator_back.py
--rw-r--r--  2.0 unx     7919 b- defN 23-Jul-09 11:29 kolibri/preprocess/timeseries/time_series_from_array.py
--rw-r--r--  2.0 unx     8504 b- defN 23-Jul-09 11:29 kolibri/preprocess/timeseries/window.py
--rw-r--r--  2.0 unx     7843 b- defN 23-Jul-09 11:29 kolibri/preprocess/timeseries/window_generator.py
--rw-r--r--  2.0 unx     2131 b- defN 23-Aug-25 14:12 kolibri/samplers/__init__.py
--rw-r--r--  2.0 unx     5095 b- defN 23-Aug-25 14:12 kolibri/samplers/auto_smpler.py
--rw-r--r--  2.0 unx     5952 b- defN 23-Aug-25 14:12 kolibri/samplers/conditional.py
--rw-r--r--  2.0 unx     2651 b- defN 23-Aug-25 14:12 kolibri/samplers/data_sampler.py
--rw-r--r--  2.0 unx     7780 b- defN 23-Aug-25 14:12 kolibri/samplers/smoteR.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/scripts/__init__.py
--rw-r--r--  2.0 unx      988 b- defN 23-Jul-09 11:29 kolibri/scripts/check_requirements.py
--rw-r--r--  2.0 unx     1284 b- defN 23-Jul-09 11:29 kolibri/scripts/install_plugin_deps.py
--rw-r--r--  2.0 unx       52 b- defN 23-Aug-21 19:28 kolibri/stopwords/__init__.py
--rw-r--r--  2.0 unx     2016 b- defN 23-Aug-21 19:28 kolibri/stopwords/stp_wrd.py
--rw-r--r--  2.0 unx      717 b- defN 23-Aug-21 19:28 kolibri/synthetic_data/__init__.py
--rw-r--r--  2.0 unx     3060 b- defN 23-Aug-21 19:28 kolibri/synthetic_data/anonymization.py
--rw-r--r--  2.0 unx    45790 b- defN 23-Aug-21 19:28 kolibri/synthetic_data/base.py
--rw-r--r--  2.0 unx    18063 b- defN 23-Aug-21 19:28 kolibri/synthetic_data/base_contraint.py
--rw-r--r--  2.0 unx    11107 b- defN 23-Aug-21 19:28 kolibri/synthetic_data/copulagan.py
--rw-r--r--  2.0 unx    14946 b- defN 23-Aug-21 19:28 kolibri/synthetic_data/copulas.py
--rw-r--r--  2.0 unx     5656 b- defN 23-Aug-21 19:28 kolibri/synthetic_data/ctgan_synthesizer.py
--rw-r--r--  2.0 unx    35479 b- defN 23-Aug-21 19:28 kolibri/synthetic_data/data_processor.py
--rw-r--r--  2.0 unx    21083 b- defN 23-Aug-21 19:28 kolibri/synthetic_data/metadata.py
--rw-r--r--  2.0 unx     7180 b- defN 23-Aug-21 19:28 kolibri/synthetic_data/single_table.py
--rw-r--r--  2.0 unx     7177 b- defN 23-Aug-21 19:28 kolibri/synthetic_data/synthcity_lib.py
--rw-r--r--  2.0 unx     3227 b- defN 23-Aug-21 19:28 kolibri/synthetic_data/synthpop.py
--rw-r--r--  2.0 unx    10163 b- defN 23-Aug-21 19:28 kolibri/synthetic_data/utils.py
--rw-r--r--  2.0 unx     1186 b- defN 23-Aug-21 19:28 kolibri/synthetic_data/benchmark/__init__.py
--rw-r--r--  2.0 unx    15188 b- defN 23-Aug-21 19:28 kolibri/synthetic_data/benchmark/benchmark.py
--rw-r--r--  2.0 unx     6638 b- defN 23-Aug-21 19:28 kolibri/synthetic_data/benchmark/data.py
--rw-r--r--  2.0 unx     3309 b- defN 23-Aug-21 19:28 kolibri/synthetic_data/benchmark/metrics.py
--rw-r--r--  2.0 unx     2241 b- defN 23-Aug-21 19:28 kolibri/synthetic_data/benchmark/ml.py
--rw-r--r--  2.0 unx     2051 b- defN 23-Aug-21 19:28 kolibri/synthetic_data/benchmark/privacy.py
--rw-r--r--  2.0 unx     6132 b- defN 23-Aug-21 19:28 kolibri/synthetic_data/benchmark/reporting.py
--rw-r--r--  2.0 unx     2239 b- defN 23-Aug-21 19:28 kolibri/synthetic_data/benchmark/utility.py
--rw-r--r--  2.0 unx     5464 b- defN 23-Aug-21 19:28 kolibri/synthetic_data/benchmark/utils.py
--rw-r--r--  2.0 unx     1063 b- defN 23-Aug-21 19:28 kolibri/synthetic_data/benchmark/synthesizers/__init__.py
--rw-r--r--  2.0 unx     2022 b- defN 23-Aug-21 19:28 kolibri/synthetic_data/benchmark/synthesizers/base.py
--rw-r--r--  2.0 unx     7232 b- defN 23-Aug-21 19:28 kolibri/synthetic_data/benchmark/synthesizers/generate.py
--rw-r--r--  2.0 unx     1337 b- defN 23-Aug-21 19:28 kolibri/synthetic_data/benchmark/synthesizers/identity.py
--rw-r--r--  2.0 unx     2114 b- defN 23-Aug-21 19:28 kolibri/synthetic_data/benchmark/synthesizers/independent.py
--rw-r--r--  2.0 unx     5641 b- defN 23-Aug-21 19:28 kolibri/synthetic_data/benchmark/synthesizers/sd.py
--rw-r--r--  2.0 unx     1665 b- defN 23-Aug-21 19:28 kolibri/synthetic_data/benchmark/synthesizers/uniform.py
--rw-r--r--  2.0 unx       67 b- defN 23-Aug-25 14:14 kolibri/task/__init__.py
--rw-r--r--  2.0 unx     7765 b- defN 23-Aug-25 14:14 kolibri/task/dnn_estimator.py
--rw-r--r--  2.0 unx      104 b- defN 23-Aug-21 19:28 kolibri/task/audio/__init__.py
--rw-r--r--  2.0 unx     9853 b- defN 23-Aug-21 19:28 kolibri/task/audio/base_model.py
--rw-r--r--  2.0 unx       75 b- defN 23-Aug-21 19:28 kolibri/task/audio/classification/__init__.py
--rw-r--r--  2.0 unx     3231 b- defN 23-Aug-21 19:28 kolibri/task/audio/classification/dnn_audio_estimator.py
--rw-r--r--  2.0 unx    10451 b- defN 23-Aug-21 19:28 kolibri/task/audio/classification/models.py
--rw-r--r--  2.0 unx      156 b- defN 23-Jul-09 11:29 kolibri/task/tabular/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/task/tabular/anomaly/__init__.py
--rw-r--r--  2.0 unx     1437 b- defN 23-Jul-09 11:29 kolibri/task/tabular/anomaly/anomaly_estimator.py
--rw-r--r--  2.0 unx    18943 b- defN 23-Jul-09 11:29 kolibri/task/tabular/anomaly/half_space_trees.py
--rw-r--r--  2.0 unx      700 b- defN 23-Jul-09 11:29 kolibri/task/tabular/anomaly/models.py
--rw-r--r--  2.0 unx      742 b- defN 23-Jul-09 11:29 kolibri/task/tabular/anomaly/one_class_anomaly_dector.py
--rw-r--r--  2.0 unx     3274 b- defN 23-Jul-09 11:29 kolibri/task/tabular/anomaly/semi_supervised_anomaly_dector.py
--rw-r--r--  2.0 unx     4617 b- defN 23-Jul-09 11:29 kolibri/task/tabular/anomaly/unsupervised_anomaly_dector.py
--rw-r--r--  2.0 unx       74 b- defN 23-Jul-09 11:29 kolibri/task/tabular/clustering/__init__.py
--rw-r--r--  2.0 unx     4518 b- defN 23-Jul-09 11:29 kolibri/task/tabular/clustering/clustering.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/task/tabular/regression/__init__.py
--rw-r--r--  2.0 unx     1748 b- defN 23-Aug-11 17:50 kolibri/task/tabular/regression/dnn_regression_estimator.py
--rw-r--r--  2.0 unx     2171 b- defN 23-Aug-25 12:29 kolibri/task/tabular/regression/sklearn_regression_estimator.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/task/tabular/rulemining/__init__.py
--rw-r--r--  2.0 unx     9912 b- defN 23-Jul-09 11:29 kolibri/task/tabular/rulemining/association_rules.py
--rw-r--r--  2.0 unx      140 b- defN 23-Aug-21 19:28 kolibri/task/text/__init__.py
--rw-r--r--  2.0 unx      190 b- defN 23-Aug-21 19:28 kolibri/task/text/classification/__init__.py
--rw-r--r--  2.0 unx     4316 b- defN 23-Aug-21 19:28 kolibri/task/text/classification/dnn_classification_estimator.py
--rw-r--r--  2.0 unx     3199 b- defN 23-Aug-21 19:28 kolibri/task/text/classification/sklearn_classification_estimator.py
--rw-r--r--  2.0 unx     3292 b- defN 23-Aug-21 19:28 kolibri/task/text/classification/sklearn_estimator.py
--rw-r--r--  2.0 unx     3145 b- defN 23-Aug-21 19:28 kolibri/task/text/entities/__init__.py
--rw-r--r--  2.0 unx     1990 b- defN 23-Aug-21 19:28 kolibri/task/text/entities/common_reg_extractor.py
--rw-r--r--  2.0 unx    17418 b- defN 23-Aug-21 19:28 kolibri/task/text/entities/crf_entity_extractor.py
--rw-r--r--  2.0 unx      949 b- defN 23-Aug-21 19:28 kolibri/task/text/entities/dictionaryExtractor.py
--rw-r--r--  2.0 unx     1111 b- defN 23-Aug-21 19:28 kolibri/task/text/entities/entity.py
--rw-r--r--  2.0 unx     3007 b- defN 23-Aug-21 19:28 kolibri/task/text/entities/entity_extractor.py
--rw-r--r--  2.0 unx     4171 b- defN 23-Aug-21 19:28 kolibri/task/text/entities/entity_synonyms.py
--rw-r--r--  2.0 unx     6339 b- defN 23-Aug-21 19:28 kolibri/task/text/entities/lstm_entity_extractor.py
--rw-r--r--  2.0 unx     3633 b- defN 23-Aug-21 19:28 kolibri/task/text/entities/person_extractor.py
--rw-r--r--  2.0 unx     2279 b- defN 23-Aug-21 19:28 kolibri/task/text/entities/preprocessing.py
--rw-r--r--  2.0 unx     2668 b- defN 23-Aug-21 19:28 kolibri/task/text/entities/regex_extractor.py
--rw-r--r--  2.0 unx     6945 b- defN 23-Aug-21 19:28 kolibri/task/text/entities/templated_extractor.py
--rw-r--r--  2.0 unx     3498 b- defN 23-Aug-21 19:28 kolibri/task/text/entities/test.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 19:28 kolibri/task/text/entities_back/__init__.py
--rw-r--r--  2.0 unx     6458 b- defN 23-Aug-21 19:28 kolibri/task/text/entities_back/common_reg_extractor.py
--rw-r--r--  2.0 unx    18309 b- defN 23-Aug-21 19:28 kolibri/task/text/entities_back/crf_entity_extractor.py
--rw-r--r--  2.0 unx     1011 b- defN 23-Aug-21 19:28 kolibri/task/text/entities_back/dictionaryExtractor.py
--rw-r--r--  2.0 unx     2997 b- defN 23-Aug-21 19:28 kolibri/task/text/entities_back/entity_extractor.py
--rw-r--r--  2.0 unx     4343 b- defN 23-Aug-21 19:28 kolibri/task/text/entities_back/entity_synonyms.py
--rw-r--r--  2.0 unx     3188 b- defN 23-Aug-21 19:28 kolibri/task/text/entities_back/person_extractor.py
--rw-r--r--  2.0 unx     2295 b- defN 23-Aug-21 19:28 kolibri/task/text/entities_back/preprocessing.py
--rw-r--r--  2.0 unx     2644 b- defN 23-Aug-21 19:28 kolibri/task/text/entities_back/regex_extractor.py
--rw-r--r--  2.0 unx     6419 b- defN 23-Aug-21 19:28 kolibri/task/text/entities_back/templated_extractor.py
--rw-r--r--  2.0 unx        5 b- defN 23-Aug-21 19:28 kolibri/task/text/intents/__init__.py
--rw-r--r--  2.0 unx    10289 b- defN 23-Aug-21 19:28 kolibri/task/text/intents/intent_catcher.py
--rw-r--r--  2.0 unx     3811 b- defN 23-Aug-21 19:28 kolibri/task/text/intents/intent_expressions.py
--rw-r--r--  2.0 unx     1437 b- defN 23-Aug-21 19:28 kolibri/task/text/intents/domains/__init__.py
--rw-r--r--  2.0 unx        1 b- defN 23-Aug-21 19:28 kolibri/task/text/sentiment/__init__.py
--rw-r--r--  2.0 unx    12971 b- defN 23-Aug-21 19:28 kolibri/task/text/sentiment/lexicon_sentiment.py
--rw-r--r--  2.0 unx    32780 b- defN 23-Aug-21 19:28 kolibri/task/text/sentiment/util.py
--rw-r--r--  2.0 unx    22769 b- defN 23-Aug-21 19:28 kolibri/task/text/sentiment/vader.py
--rw-r--r--  2.0 unx     2587 b- defN 23-Aug-21 19:28 kolibri/task/text/similarity/__init__.py
--rw-r--r--  2.0 unx      559 b- defN 23-Aug-21 19:28 kolibri/task/text/similarity/arxiv.py
--rw-r--r--  2.0 unx     6717 b- defN 23-Aug-21 19:28 kolibri/task/text/similarity/docarray.py
--rw-r--r--  2.0 unx     2361 b- defN 23-Aug-21 19:28 kolibri/task/text/similarity/knn.py
--rw-r--r--  2.0 unx     2907 b- defN 23-Aug-21 19:28 kolibri/task/text/similarity/llama_index.py
--rw-r--r--  2.0 unx     2907 b- defN 23-Aug-21 19:28 kolibri/task/text/similarity/merger_retriever.py
--rw-r--r--  2.0 unx      569 b- defN 23-Aug-21 19:28 kolibri/task/text/similarity/pupmed.py
--rw-r--r--  2.0 unx     2953 b- defN 23-Aug-21 19:28 kolibri/task/text/similarity/svm.py
--rw-r--r--  2.0 unx     2470 b- defN 23-Aug-21 19:28 kolibri/task/text/similarity/tfidf.py
--rw-r--r--  2.0 unx      579 b- defN 23-Aug-21 19:28 kolibri/task/text/similarity/wikipedia.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 19:28 kolibri/task/text/spelling/__init__.py
--rw-r--r--  2.0 unx       36 b- defN 23-Aug-21 19:28 kolibri/task/text/spelling/brillmoore/__init__.py
--rw-r--r--  2.0 unx    10769 b- defN 23-Aug-21 19:28 kolibri/task/text/spelling/brillmoore/error_model.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 19:28 kolibri/task/text/spelling/electors/__init__.py
--rw-r--r--  2.0 unx     2815 b- defN 23-Aug-21 19:28 kolibri/task/text/spelling/electors/kenlm_elector.py
--rw-r--r--  2.0 unx     1421 b- defN 23-Aug-21 19:28 kolibri/task/text/spelling/electors/top1_elector.py
--rw-r--r--  2.0 unx       61 b- defN 23-Aug-21 19:28 kolibri/task/text/spelling/levenshtein/__init__.py
--rw-r--r--  2.0 unx    33386 b- defN 23-Aug-21 19:28 kolibri/task/text/spelling/levenshtein/levenshtein_searcher.py
--rw-r--r--  2.0 unx     3406 b- defN 23-Aug-21 19:28 kolibri/task/text/spelling/levenshtein/searcher_component.py
--rw-r--r--  2.0 unx    20586 b- defN 23-Aug-21 19:28 kolibri/task/text/spelling/levenshtein/tabled_trie.py
--rw-r--r--  2.0 unx      152 b- defN 23-Aug-21 19:28 kolibri/task/text/topics/__init__.py
--rw-r--r--  2.0 unx     3563 b- defN 23-Aug-21 19:28 kolibri/task/text/topics/baseTopic.py
--rw-r--r--  2.0 unx    24958 b- defN 23-Aug-21 19:28 kolibri/task/text/topics/mallet.py
--rw-r--r--  2.0 unx    14855 b- defN 23-Aug-21 19:28 kolibri/task/text/topics/topics_estimator.py
--rw-r--r--  2.0 unx       58 b- defN 23-Jul-09 11:29 kolibri/task/timeseries/__init__.py
--rw-r--r--  2.0 unx    23782 b- defN 23-Jul-09 11:29 kolibri/task/timeseries/dataset.py
--rw-r--r--  2.0 unx      962 b- defN 23-Jul-09 11:29 kolibri/task/timeseries/metrics.py
--rw-r--r--  2.0 unx     1953 b- defN 23-Jul-09 11:29 kolibri/task/timeseries/analysis/__init__.py
--rw-r--r--  2.0 unx     7234 b- defN 23-Jul-09 11:29 kolibri/task/timeseries/analysis/eda_utils.py
--rw-r--r--  2.0 unx    17003 b- defN 23-Jul-09 11:29 kolibri/task/timeseries/analysis/plotters.py
--rw-r--r--  2.0 unx      494 b- defN 23-Jul-09 11:29 kolibri/task/timeseries/analysis/feature_relevance/__init__.py
--rw-r--r--  2.0 unx     3066 b- defN 23-Jul-09 11:29 kolibri/task/timeseries/analysis/feature_relevance/relevance.py
--rw-r--r--  2.0 unx     2919 b- defN 23-Jul-09 11:29 kolibri/task/timeseries/analysis/feature_relevance/relevance_table.py
--rw-r--r--  2.0 unx      583 b- defN 23-Jul-09 11:29 kolibri/task/timeseries/analysis/outliers/__init__.py
--rw-r--r--  2.0 unx     5017 b- defN 23-Jul-09 11:29 kolibri/task/timeseries/analysis/outliers/density_outliers.py
--rw-r--r--  2.0 unx    13178 b- defN 23-Jul-09 11:29 kolibri/task/timeseries/analysis/outliers/hist_outliers.py
--rw-r--r--  2.0 unx     1878 b- defN 23-Jul-09 11:29 kolibri/task/timeseries/analysis/outliers/median_outliers.py
--rw-r--r--  2.0 unx     2998 b- defN 23-Jul-09 11:29 kolibri/task/timeseries/analysis/outliers/prediction_interval_outliers.py
--rw-r--r--  2.0 unx     3501 b- defN 23-Jul-09 11:29 kolibri/task/timeseries/analysis/outliers/sequence_outliers.py
--rw-r--r--  2.0 unx     1470 b- defN 23-Aug-21 19:28 kolibri/tokenizers/__init__.py
--rw-r--r--  2.0 unx     4690 b- defN 23-Aug-21 19:28 kolibri/tokenizers/bert_tokenizer.py
--rw-r--r--  2.0 unx     3999 b- defN 23-Aug-21 19:28 kolibri/tokenizers/char_tokenizer.py
--rw-r--r--  2.0 unx     7103 b- defN 23-Aug-21 19:28 kolibri/tokenizers/kolibri_tokenizer.py
--rw-r--r--  2.0 unx     2361 b- defN 23-Aug-21 19:28 kolibri/tokenizers/multi_word_tokenizer.py
--rw-r--r--  2.0 unx     2661 b- defN 23-Aug-21 19:28 kolibri/tokenizers/regex_tokenizer.py
--rw-r--r--  2.0 unx     1025 b- defN 23-Aug-21 19:28 kolibri/tokenizers/sentence_tokenizer.py
--rw-r--r--  2.0 unx     2708 b- defN 23-Aug-21 19:28 kolibri/tokenizers/tokenizer.py
--rw-r--r--  2.0 unx     6936 b- defN 23-Aug-21 19:28 kolibri/tokenizers/ugc_tokenizer.py
--rw-r--r--  2.0 unx     2404 b- defN 23-Aug-21 19:28 kolibri/tokenizers/word_tokenizer.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-21 19:28 kolibri/tools/__init__.py
--rw-r--r--  2.0 unx      411 b- defN 23-Aug-21 19:28 kolibri/tools/_regex.py
--rw-r--r--  2.0 unx      841 b- defN 23-Aug-21 19:28 kolibri/tools/arxiv.py
--rw-r--r--  2.0 unx     1208 b- defN 23-Aug-21 19:28 kolibri/tools/bing_search.py
--rw-r--r--  2.0 unx     1441 b- defN 23-Aug-21 19:28 kolibri/tools/ddg_search.py
--rw-r--r--  2.0 unx     2063 b- defN 23-Aug-21 19:28 kolibri/tools/gebbrisg_detector.py
--rw-r--r--  2.0 unx     1231 b- defN 23-Aug-21 19:28 kolibri/tools/google_search.py
--rw-r--r--  2.0 unx    25525 b- defN 23-Aug-21 19:28 kolibri/tools/keywords.py
--rw-r--r--  2.0 unx      777 b- defN 23-Aug-21 19:28 kolibri/tools/openweathermap.py
--rw-r--r--  2.0 unx      853 b- defN 23-Aug-21 19:28 kolibri/tools/pubmed.py
--rw-r--r--  2.0 unx     1828 b- defN 23-Aug-21 19:28 kolibri/tools/regexes.py
--rw-r--r--  2.0 unx    17263 b- defN 23-Aug-21 19:28 kolibri/tools/scanner.py
--rw-r--r--  2.0 unx      690 b- defN 23-Aug-21 19:28 kolibri/tools/wikipedia.py
--rw-r--r--  2.0 unx      699 b- defN 23-Aug-21 19:28 kolibri/tools/wolfram_alpha.py
--rw-r--r--  2.0 unx    13056 b- defN 23-Aug-21 19:28 kolibri/tools/word_frequencies.py
--rw-r--r--  2.0 unx     1447 b- defN 23-Aug-21 19:28 kolibri/tools/youtube_search.py
--rw-r--r--  2.0 unx     5493 b- defN 23-Aug-25 14:14 kolibri/utils/__init__.py
--rw-r--r--  2.0 unx    11199 b- defN 23-Aug-25 14:14 kolibri/utils/cm.py
--rw-r--r--  2.0 unx     6904 b- defN 23-Jul-09 11:29 kolibri/utils/common.py
--rw-r--r--  2.0 unx     3173 b- defN 23-Jul-09 11:29 kolibri/utils/config.py
--rw-r--r--  2.0 unx    12009 b- defN 23-Jul-09 11:29 kolibri/utils/cross_validation.py
--rw-r--r--  2.0 unx    14474 b- defN 23-Jul-09 11:29 kolibri/utils/distribution.py
--rw-r--r--  2.0 unx      873 b- defN 23-Jul-09 11:29 kolibri/utils/environement.py
--rw-r--r--  2.0 unx     3259 b- defN 23-Jul-09 11:29 kolibri/utils/language_info.py
--rw-r--r--  2.0 unx      544 b- defN 23-Jul-09 11:29 kolibri/utils/log_normalizer.py
--rw-r--r--  2.0 unx     5686 b- defN 23-Jul-09 11:29 kolibri/utils/mathext.py
--rw-r--r--  2.0 unx     2904 b- defN 23-Jul-09 11:29 kolibri/utils/matrix.py
--rw-r--r--  2.0 unx     3158 b- defN 23-Jul-09 11:29 kolibri/utils/nb_clusters.py
--rw-r--r--  2.0 unx      631 b- defN 23-Jul-09 11:29 kolibri/utils/parallel.py
--rw-r--r--  2.0 unx     2361 b- defN 23-Jul-09 11:29 kolibri/utils/progress_bar.py
--rw-r--r--  2.0 unx     4577 b- defN 23-Aug-25 14:14 kolibri/utils/serializable.py
--rw-r--r--  2.0 unx     2280 b- defN 23-Jul-09 11:29 kolibri/utils/spinner.py
--rw-r--r--  2.0 unx     1252 b- defN 23-Jul-09 11:29 kolibri/utils/text_encoding.py
--rw-r--r--  2.0 unx    28893 b- defN 23-Jul-09 11:29 kolibri/utils/timeseries_functions.py
--rw-r--r--  2.0 unx    28840 b- defN 23-Jul-09 11:29 kolibri/utils/timeseries_functions_back.py
--rw-r--r--  2.0 unx      547 b- defN 23-Aug-21 19:28 kolibri/utils/wrappers/__init__.py
--rw-r--r--  2.0 unx     5589 b- defN 23-Aug-21 19:28 kolibri/utils/wrappers/arxiv.py
--rw-r--r--  2.0 unx     3344 b- defN 23-Aug-21 19:28 kolibri/utils/wrappers/bing_search.py
--rw-r--r--  2.0 unx     3330 b- defN 23-Aug-21 19:28 kolibri/utils/wrappers/duckduckgo_search.py
--rw-r--r--  2.0 unx     4910 b- defN 23-Aug-21 19:28 kolibri/utils/wrappers/google_search.py
--rw-r--r--  2.0 unx     2431 b- defN 23-Aug-21 19:28 kolibri/utils/wrappers/openweathermap.py
--rw-r--r--  2.0 unx     5742 b- defN 23-Aug-21 19:28 kolibri/utils/wrappers/pupmed.py
--rw-r--r--  2.0 unx     4035 b- defN 23-Aug-21 19:28 kolibri/utils/wrappers/wikipedia.py
--rw-r--r--  2.0 unx     2000 b- defN 23-Aug-21 19:28 kolibri/utils/wrappers/wolfram_alpha.py
--rw-r--r--  2.0 unx      347 b- defN 23-Aug-21 19:28 kolibri/vectordb/__init__.py
--rw-r--r--  2.0 unx    16307 b- defN 23-Aug-21 19:28 kolibri/vectordb/base.py
--rw-r--r--  2.0 unx    23410 b- defN 23-Aug-21 19:28 kolibri/vectordb/faiss.py
--rw-r--r--  2.0 unx    21812 b- defN 23-Aug-21 19:28 kolibri/vectordb/redis.py
--rw-r--r--  2.0 unx    12276 b- defN 23-Aug-21 19:28 kolibri/vectordb/sklearn.py
--rw-r--r--  2.0 unx     1462 b- defN 23-Aug-21 19:28 kolibri/vectordb/utils.py
--rw-r--r--  2.0 unx      204 b- defN 23-Aug-21 19:28 kolibri/vectordb/docarray/__init__.py
--rw-r--r--  2.0 unx     6872 b- defN 23-Aug-21 19:28 kolibri/vectordb/docarray/base.py
--rw-r--r--  2.0 unx     4062 b- defN 23-Aug-21 19:28 kolibri/vectordb/docarray/hnsw.py
--rw-r--r--  2.0 unx     2416 b- defN 23-Aug-21 19:28 kolibri/vectordb/docarray/in_memory.py
--rw-r--r--  2.0 unx      280 b- defN 23-Aug-21 19:28 kolibri/vectordb/docstore/__init__.py
--rw-r--r--  2.0 unx      924 b- defN 23-Aug-21 19:28 kolibri/vectordb/docstore/arbitrary_fn.py
--rw-r--r--  2.0 unx      694 b- defN 23-Aug-21 19:28 kolibri/vectordb/docstore/base.py
--rw-r--r--  2.0 unx      973 b- defN 23-Aug-21 19:28 kolibri/vectordb/docstore/in_memory.py
--rw-r--r--  2.0 unx     1376 b- defN 23-Aug-21 19:28 kolibri/vectordb/docstore/wikipedia.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/visualizations/__init__.py
--rw-r--r--  2.0 unx    53414 b- defN 23-Aug-25 14:14 kolibri/visualizations/classification_plots.py
--rw-r--r--  2.0 unx    15746 b- defN 23-Jul-09 11:29 kolibri/visualizations/pipeline.py
--rw-r--r--  2.0 unx    34807 b- defN 23-Aug-25 15:10 kolibri/visualizations/regression_plots.py
--rw-r--r--  2.0 unx    15565 b- defN 23-Jul-09 11:29 kolibri/visualizations/utils.py
+Zip file size: 1685116 bytes, number of entries: 780
+-rw-r--r--  2.0 unx        5 b- defN 24-Apr-08 23:01 kolibri/VERSION
+-rw-r--r--  2.0 unx     4514 b- defN 24-Apr-08 20:27 kolibri/__init__.py
+-rw-r--r--  2.0 unx    16782 b- defN 24-Apr-06 12:47 kolibri/app.py
+-rw-r--r--  2.0 unx     3190 b- defN 24-Apr-06 12:47 kolibri/config.py
+-rw-r--r--  2.0 unx     1902 b- defN 24-Apr-06 12:47 kolibri/config_loader.py
+-rw-r--r--  2.0 unx     3814 b- defN 24-Apr-06 12:47 kolibri/default_configs.py
+-rw-r--r--  2.0 unx     5968 b- defN 24-Apr-06 12:47 kolibri/errors.py
+-rw-r--r--  2.0 unx      795 b- defN 24-Apr-06 12:47 kolibri/logger.py
+-rw-r--r--  2.0 unx     2219 b- defN 24-Apr-06 12:47 kolibri/metadata.py
+-rw-r--r--  2.0 unx    10923 b- defN 24-Apr-06 12:47 kolibri/model_loader.py
+-rw-r--r--  2.0 unx    26008 b- defN 24-Apr-06 13:58 kolibri/model_trainer.py
+-rw-r--r--  2.0 unx     2763 b- defN 24-Apr-06 12:47 kolibri/registry.py
+-rw-r--r--  2.0 unx      153 b- defN 24-Apr-06 12:47 kolibri/requirements.txt
+-rw-r--r--  2.0 unx     2490 b- defN 24-Apr-06 12:47 kolibri/settings.py
+-rw-r--r--  2.0 unx      457 b- defN 24-Apr-06 12:47 kolibri/settings.yaml
+-rw-r--r--  2.0 unx      361 b- defN 24-Apr-06 12:47 kolibri/types.py
+-rw-r--r--  2.0 unx      166 b- defN 24-Apr-06 12:47 kolibri/version.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 12:47 kolibri/api/__init__.py
+-rw-r--r--  2.0 unx     2707 b- defN 24-Apr-06 12:47 kolibri/api/classification/__init__.py
+-rw-r--r--  2.0 unx       66 b- defN 24-Apr-06 12:47 kolibri/autolearn/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 12:47 kolibri/autolearn/metalearn/__init__.py
+-rw-r--r--  2.0 unx     3125 b- defN 24-Apr-06 12:47 kolibri/autolearn/metalearn/metafeature.py
+-rw-r--r--  2.0 unx    46866 b- defN 24-Apr-06 12:47 kolibri/autolearn/metalearn/metafeatures.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 12:47 kolibri/autolearn/model_zoo/__init__.py
+-rw-r--r--  2.0 unx     4781 b- defN 24-Apr-06 13:50 kolibri/autolearn/model_zoo/zoo_classifier.py
+-rw-r--r--  2.0 unx     5834 b- defN 24-Apr-06 12:47 kolibri/autolearn/model_zoo/zoo_estimator.py
+-rw-r--r--  2.0 unx     4246 b- defN 24-Apr-06 12:47 kolibri/autolearn/model_zoo/zoo_regressor.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 12:47 kolibri/automl/__init__.py
+-rw-r--r--  2.0 unx    15341 b- defN 24-Apr-06 12:47 kolibri/automl/data_inspection.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 12:47 kolibri/backend/__init__.py
+-rw-r--r--  2.0 unx     6230 b- defN 24-Apr-06 12:47 kolibri/backend/models.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 12:47 kolibri/backend/base/__init__.py
+-rw-r--r--  2.0 unx    11830 b- defN 24-Apr-06 13:46 kolibri/backend/base/base_classifier.py
+-rw-r--r--  2.0 unx     3916 b- defN 24-Apr-06 12:47 kolibri/backend/base/base_clustering.py
+-rw-r--r--  2.0 unx    30807 b- defN 24-Apr-06 13:20 kolibri/backend/base/base_estimator.py
+-rw-r--r--  2.0 unx     7418 b- defN 24-Apr-06 12:47 kolibri/backend/base/base_regressor.py
+-rw-r--r--  2.0 unx    14321 b- defN 24-Apr-06 12:47 kolibri/backend/base/estimator.py
+-rw-r--r--  2.0 unx      912 b- defN 24-Apr-06 12:47 kolibri/backend/base/nn_model.py
+-rw-r--r--  2.0 unx      148 b- defN 24-Mar-31 15:44 kolibri/backend/bert4keras/__init__.py
+-rw-r--r--  2.0 unx    20228 b- defN 24-Mar-31 15:44 kolibri/backend/bert4keras/backend.py
+-rw-r--r--  2.0 unx    52339 b- defN 24-Mar-31 15:44 kolibri/backend/bert4keras/layers.py
+-rw-r--r--  2.0 unx   123662 b- defN 24-Mar-31 15:44 kolibri/backend/bert4keras/models.py
+-rw-r--r--  2.0 unx    30152 b- defN 24-Mar-31 13:10 kolibri/backend/bert4keras/ops.py
+-rw-r--r--  2.0 unx    27957 b- defN 24-Apr-05 10:56 kolibri/backend/bert4keras/snippets.py
+-rw-r--r--  2.0 unx    15504 b- defN 24-Mar-31 15:44 kolibri/backend/bert4keras/tokenizers.py
+-rw-r--r--  2.0 unx      449 b- defN 24-Apr-06 12:47 kolibri/backend/bn/BayesianModel.py
+-rw-r--r--  2.0 unx    44071 b- defN 24-Apr-06 12:47 kolibri/backend/bn/BayesianNetwork.py
+-rw-r--r--  2.0 unx    24029 b- defN 24-Apr-06 12:47 kolibri/backend/bn/CPD.py
+-rw-r--r--  2.0 unx     8931 b- defN 24-Apr-06 12:47 kolibri/backend/bn/ContinuousFactor.py
+-rw-r--r--  2.0 unx    40531 b- defN 24-Apr-06 12:47 kolibri/backend/bn/DAG.py
+-rw-r--r--  2.0 unx    28630 b- defN 24-Apr-06 12:47 kolibri/backend/bn/DiscreteFactor.py
+-rw-r--r--  2.0 unx    31370 b- defN 24-Apr-06 12:47 kolibri/backend/bn/DynamicBayesianNetwork.py
+-rw-r--r--  2.0 unx     4289 b- defN 24-Apr-06 12:47 kolibri/backend/bn/EliminationOrder.py
+-rw-r--r--  2.0 unx    39930 b- defN 24-Apr-06 12:47 kolibri/backend/bn/ExactInference.py
+-rw-r--r--  2.0 unx    10515 b- defN 24-Apr-06 12:47 kolibri/backend/bn/FactorGraph.py
+-rw-r--r--  2.0 unx    14252 b- defN 24-Apr-06 12:47 kolibri/backend/bn/Independencies.py
+-rw-r--r--  2.0 unx    11089 b- defN 24-Apr-06 12:47 kolibri/backend/bn/JointProbabilityDistribution.py
+-rw-r--r--  2.0 unx     3058 b- defN 24-Apr-06 12:47 kolibri/backend/bn/JunctionTree.py
+-rw-r--r--  2.0 unx     8219 b- defN 24-Apr-06 12:47 kolibri/backend/bn/LinearGaussianCPD.py
+-rw-r--r--  2.0 unx    13783 b- defN 24-Apr-06 12:47 kolibri/backend/bn/MarkovChain.py
+-rw-r--r--  2.0 unx    17804 b- defN 24-Apr-06 12:47 kolibri/backend/bn/MarkovNetwork.py
+-rw-r--r--  2.0 unx     5791 b- defN 24-Apr-06 12:47 kolibri/backend/bn/NaiveBayes.py
+-rw-r--r--  2.0 unx    24083 b- defN 24-Apr-06 12:47 kolibri/backend/bn/Sampling.py
+-rw-r--r--  2.0 unx     9237 b- defN 24-Apr-06 12:47 kolibri/backend/bn/UndirectedGraph.py
+-rw-r--r--  2.0 unx      723 b- defN 24-Apr-06 12:47 kolibri/backend/bn/__init__.py
+-rw-r--r--  2.0 unx    11145 b- defN 24-Apr-06 12:47 kolibri/backend/bn/base_estimator.py
+-rw-r--r--  2.0 unx     7604 b- defN 24-Apr-06 12:47 kolibri/backend/bn/base_inference.py
+-rw-r--r--  2.0 unx    48040 b- defN 24-Apr-06 12:47 kolibri/backend/bn/bnlearn.py
+-rw-r--r--  2.0 unx     3207 b- defN 24-Apr-06 12:47 kolibri/backend/bn/factors_base.py
+-rw-r--r--  2.0 unx     2348 b- defN 24-Apr-06 12:47 kolibri/backend/bn/metrics.py
+-rw-r--r--  2.0 unx    12326 b- defN 24-Apr-06 12:47 kolibri/backend/bn/network.py
+-rw-r--r--  2.0 unx     3178 b- defN 24-Apr-06 12:47 kolibri/backend/bn/state_name.py
+-rw-r--r--  2.0 unx    30222 b- defN 24-Apr-06 12:47 kolibri/backend/bn/tabulate.py
+-rw-r--r--  2.0 unx     5326 b- defN 24-Apr-06 12:47 kolibri/backend/bn/utils.py
+-rw-r--r--  2.0 unx    13476 b- defN 24-Apr-06 12:47 kolibri/backend/bn/distributions/CanonicalDistribution.py
+-rw-r--r--  2.0 unx    11847 b- defN 24-Apr-06 12:47 kolibri/backend/bn/distributions/CustomDistribution.py
+-rw-r--r--  2.0 unx    19195 b- defN 24-Apr-06 12:47 kolibri/backend/bn/distributions/GaussianDistribution.py
+-rw-r--r--  2.0 unx      220 b- defN 24-Apr-06 12:47 kolibri/backend/bn/distributions/__init__.py
+-rw-r--r--  2.0 unx      841 b- defN 24-Apr-06 12:47 kolibri/backend/bn/distributions/base.py
+-rw-r--r--  2.0 unx    12715 b- defN 24-Apr-06 12:47 kolibri/backend/bn/estimators/HillClimbSearch.py
+-rw-r--r--  2.0 unx     4805 b- defN 24-Apr-06 12:47 kolibri/backend/bn/estimators/MLE.py
+-rw-r--r--  2.0 unx     4221 b- defN 24-Apr-06 12:47 kolibri/backend/bn/estimators/ScoreCache.py
+-rw-r--r--  2.0 unx    18012 b- defN 24-Apr-06 12:47 kolibri/backend/bn/estimators/StructureScore.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 12:47 kolibri/backend/bn/estimators/__init__.py
+-rw-r--r--  2.0 unx     7985 b- defN 24-Apr-06 12:47 kolibri/backend/bn/estimators/bayesianEstimator.py
+-rw-r--r--  2.0 unx       57 b- defN 24-Apr-06 12:47 kolibri/backend/bn/inference/__init__.py
+-rw-r--r--  2.0 unx     3044 b- defN 24-Apr-06 12:47 kolibri/backend/bn/inference/inference.py
+-rw-r--r--  2.0 unx      194 b- defN 24-Apr-06 12:47 kolibri/backend/bn/inference/predict.py
+-rw-r--r--  2.0 unx      130 b- defN 24-Apr-06 12:47 kolibri/backend/bn/parameters/__init__.py
+-rw-r--r--  2.0 unx      490 b- defN 24-Apr-06 12:47 kolibri/backend/bn/parameters/learn.py
+-rw-r--r--  2.0 unx    12213 b- defN 24-Apr-06 12:47 kolibri/backend/bn/parameters/parameter_learning.py
+-rw-r--r--  2.0 unx    18288 b- defN 24-Apr-06 12:47 kolibri/backend/bn/readwrite/BIF.py
+-rw-r--r--  2.0 unx    14034 b- defN 24-Apr-06 12:47 kolibri/backend/bn/readwrite/UAI.py
+-rw-r--r--  2.0 unx    16390 b- defN 24-Apr-06 12:47 kolibri/backend/bn/readwrite/XMLBIF.py
+-rw-r--r--  2.0 unx      491 b- defN 24-Apr-06 12:47 kolibri/backend/bn/readwrite/__init__.py
+-rw-r--r--  2.0 unx      311 b- defN 24-Apr-06 12:47 kolibri/backend/bn/structure/__init__.py
+-rw-r--r--  2.0 unx     7020 b- defN 24-Apr-06 12:47 kolibri/backend/bn/structure/base.py
+-rw-r--r--  2.0 unx     8354 b- defN 24-Apr-06 12:47 kolibri/backend/bn/structure/evaluation.py
+-rw-r--r--  2.0 unx     1989 b- defN 24-Apr-06 12:47 kolibri/backend/bn/structure/learn.py
+-rw-r--r--  2.0 unx     7267 b- defN 24-Apr-06 12:47 kolibri/backend/bn/structure/linear.py
+-rw-r--r--  2.0 unx     7902 b- defN 24-Apr-06 12:47 kolibri/backend/bn/structure/low_rank.py
+-rw-r--r--  2.0 unx    22607 b- defN 24-Apr-06 12:47 kolibri/backend/bn/structure/no_tears.py
+-rw-r--r--  2.0 unx     2961 b- defN 24-Apr-06 12:47 kolibri/backend/bn/structure/no_tears_tf.py
+-rw-r--r--  2.0 unx     1898 b- defN 24-Apr-06 12:47 kolibri/backend/bn/structure/no_tears_tf2.py
+-rw-r--r--  2.0 unx     2961 b- defN 24-Apr-06 12:47 kolibri/backend/bn/structure/no_tears_tf_bak.py
+-rw-r--r--  2.0 unx     8820 b- defN 24-Apr-08 20:26 kolibri/backend/bn/structure/nonlinear.py
+-rw-r--r--  2.0 unx     4376 b- defN 24-Apr-06 12:47 kolibri/backend/bn/structure/notears_tf2.py
+-rw-r--r--  2.0 unx     4208 b- defN 24-Apr-06 12:47 kolibri/backend/bn/structure/plot_dag.py
+-rw-r--r--  2.0 unx    13671 b- defN 24-Apr-06 12:47 kolibri/backend/bn/structure/structure_model.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 12:47 kolibri/backend/generators/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-05 08:49 kolibri/backend/model_abstractions/__init__.py
+-rw-r--r--  2.0 unx     7922 b- defN 24-Apr-05 10:17 kolibri/backend/model_abstractions/model_object.py
+-rw-r--r--  2.0 unx     3106 b- defN 24-Apr-05 13:42 kolibri/backend/model_abstractions/model_params.py
+-rw-r--r--  2.0 unx     2611 b- defN 24-Apr-08 20:27 kolibri/backend/pytorch/__init__.py
+-rw-r--r--  2.0 unx      618 b- defN 24-Apr-02 15:34 kolibri/backend/pytorch/class_utils.py
+-rw-r--r--  2.0 unx    69867 b- defN 24-Apr-08 22:12 kolibri/backend/pytorch/data.py
+-rw-r--r--  2.0 unx    13971 b- defN 24-Apr-08 20:27 kolibri/backend/pytorch/file_utils.py
+-rw-r--r--  2.0 unx    12239 b- defN 24-Apr-08 20:31 kolibri/backend/pytorch/inference_utils.py
+-rw-r--r--  2.0 unx    10900 b- defN 24-Apr-08 15:04 kolibri/backend/pytorch/optim.py
+-rw-r--r--  2.0 unx     3674 b- defN 24-Apr-08 15:04 kolibri/backend/pytorch/samplers.py
+-rw-r--r--  2.0 unx     8216 b- defN 24-Apr-08 20:26 kolibri/backend/pytorch/splitter.py
+-rw-r--r--  2.0 unx     9749 b- defN 24-Apr-08 15:04 kolibri/backend/pytorch/tokenization.py
+-rw-r--r--  2.0 unx    14087 b- defN 24-Apr-08 20:31 kolibri/backend/pytorch/training_utils.py
+-rw-r--r--  2.0 unx     4333 b- defN 24-Apr-08 10:03 kolibri/backend/pytorch/datasets/__init__.py
+-rw-r--r--  2.0 unx     9448 b- defN 24-Apr-08 20:26 kolibri/backend/pytorch/datasets/base.py
+-rw-r--r--  2.0 unx    91543 b- defN 24-Apr-08 20:28 kolibri/backend/pytorch/datasets/document_classification.py
+-rw-r--r--  2.0 unx   202979 b- defN 24-Apr-08 20:28 kolibri/backend/pytorch/datasets/sequence_labeling.py
+-rw-r--r--  2.0 unx     2473 b- defN 24-Apr-08 20:26 kolibri/backend/pytorch/embeddings/__init__.py
+-rw-r--r--  2.0 unx     8074 b- defN 24-Apr-08 20:28 kolibri/backend/pytorch/embeddings/base.py
+-rw-r--r--  2.0 unx    30840 b- defN 24-Apr-08 20:29 kolibri/backend/pytorch/embeddings/document.py
+-rw-r--r--  2.0 unx    10954 b- defN 24-Apr-08 20:29 kolibri/backend/pytorch/embeddings/image.py
+-rw-r--r--  2.0 unx    29250 b- defN 24-Apr-08 20:30 kolibri/backend/pytorch/embeddings/legacy.py
+-rw-r--r--  2.0 unx    66585 b- defN 24-Apr-08 20:29 kolibri/backend/pytorch/embeddings/token.py
+-rw-r--r--  2.0 unx    63311 b- defN 24-Apr-08 20:28 kolibri/backend/pytorch/embeddings/transformer.py
+-rw-r--r--  2.0 unx      962 b- defN 24-Apr-08 20:24 kolibri/backend/pytorch/models/__init__.py
+-rw-r--r--  2.0 unx     4416 b- defN 24-Apr-08 20:26 kolibri/backend/pytorch/models/clustering.py
+-rw-r--r--  2.0 unx    10614 b- defN 24-Apr-08 20:26 kolibri/backend/pytorch/models/entity_linker_model.py
+-rw-r--r--  2.0 unx    17176 b- defN 24-Apr-08 20:31 kolibri/backend/pytorch/models/language_model.py
+-rw-r--r--  2.0 unx    11042 b- defN 24-Apr-08 20:34 kolibri/backend/pytorch/models/multitask_model.py
+-rw-r--r--  2.0 unx     5672 b- defN 24-Apr-08 20:43 kolibri/backend/pytorch/models/pairwise_classification_model.py
+-rw-r--r--  2.0 unx    14086 b- defN 24-Apr-08 20:44 kolibri/backend/pytorch/models/pairwise_regression_model.py
+-rw-r--r--  2.0 unx    13839 b- defN 24-Apr-08 20:26 kolibri/backend/pytorch/models/prefixed_tagger.py
+-rw-r--r--  2.0 unx     4987 b- defN 24-Apr-08 20:26 kolibri/backend/pytorch/models/regexp_tagger.py
+-rw-r--r--  2.0 unx    44679 b- defN 24-Apr-08 20:45 kolibri/backend/pytorch/models/sequence_tagger_model.py
+-rw-r--r--  2.0 unx    41492 b- defN 24-Apr-08 20:48 kolibri/backend/pytorch/models/tars_model.py
+-rw-r--r--  2.0 unx     5241 b- defN 24-Apr-08 20:46 kolibri/backend/pytorch/models/text_classification_model.py
+-rw-r--r--  2.0 unx     9594 b- defN 24-Apr-08 20:48 kolibri/backend/pytorch/models/text_regression_model.py
+-rw-r--r--  2.0 unx     9898 b- defN 24-Apr-08 20:49 kolibri/backend/pytorch/models/word_tagger_model.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-02 15:34 kolibri/backend/pytorch/models/sequence_tagger_utils/__init__.py
+-rw-r--r--  2.0 unx     2216 b- defN 24-Apr-08 20:31 kolibri/backend/pytorch/models/sequence_tagger_utils/crf.py
+-rw-r--r--  2.0 unx    11636 b- defN 24-Apr-08 20:31 kolibri/backend/pytorch/models/sequence_tagger_utils/viterbi.py
+-rw-r--r--  2.0 unx      337 b- defN 24-Apr-02 15:34 kolibri/backend/pytorch/nn/__init__.py
+-rw-r--r--  2.0 unx     8788 b- defN 24-Apr-08 20:31 kolibri/backend/pytorch/nn/decoder.py
+-rw-r--r--  2.0 unx     1747 b- defN 24-Apr-02 15:34 kolibri/backend/pytorch/nn/dropout.py
+-rw-r--r--  2.0 unx    42491 b- defN 24-Apr-08 20:31 kolibri/backend/pytorch/nn/model.py
+-rw-r--r--  2.0 unx      815 b- defN 24-Apr-08 20:26 kolibri/backend/pytorch/nn/multitask.py
+-rw-r--r--  2.0 unx      437 b- defN 24-Apr-02 15:34 kolibri/backend/pytorch/nn/recurrent.py
+-rw-r--r--  2.0 unx      387 b- defN 24-Apr-02 15:34 kolibri/backend/pytorch/nn/distance/__init__.py
+-rw-r--r--  2.0 unx     1191 b- defN 24-Apr-02 15:34 kolibri/backend/pytorch/nn/distance/cosine.py
+-rw-r--r--  2.0 unx     1838 b- defN 24-Apr-02 15:34 kolibri/backend/pytorch/nn/distance/euclidean.py
+-rw-r--r--  2.0 unx     3718 b- defN 24-Apr-02 15:34 kolibri/backend/pytorch/nn/distance/hyperbolic.py
+-rw-r--r--  2.0 unx      169 b- defN 24-Apr-02 15:34 kolibri/backend/pytorch/trainers/__init__.py
+-rw-r--r--  2.0 unx    17302 b- defN 24-Apr-08 20:31 kolibri/backend/pytorch/trainers/language_model_trainer.py
+-rw-r--r--  2.0 unx    39933 b- defN 24-Apr-08 20:50 kolibri/backend/pytorch/trainers/trainer.py
+-rw-r--r--  2.0 unx     1092 b- defN 24-Apr-02 15:34 kolibri/backend/pytorch/trainers/plugins/__init__.py
+-rw-r--r--  2.0 unx     8498 b- defN 24-Apr-08 15:04 kolibri/backend/pytorch/trainers/plugins/base.py
+-rw-r--r--  2.0 unx     4386 b- defN 24-Apr-02 15:34 kolibri/backend/pytorch/trainers/plugins/metric_records.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-02 15:34 kolibri/backend/pytorch/trainers/plugins/functional/__init__.py
+-rw-r--r--  2.0 unx     4279 b- defN 24-Apr-08 20:26 kolibri/backend/pytorch/trainers/plugins/functional/anneal_on_plateau.py
+-rw-r--r--  2.0 unx     1340 b- defN 24-Apr-08 20:26 kolibri/backend/pytorch/trainers/plugins/functional/checkpoints.py
+-rw-r--r--  2.0 unx     2389 b- defN 24-Apr-08 20:26 kolibri/backend/pytorch/trainers/plugins/functional/linear_scheduler.py
+-rw-r--r--  2.0 unx     3149 b- defN 24-Apr-08 20:26 kolibri/backend/pytorch/trainers/plugins/functional/reduce_transformer_vocab.py
+-rw-r--r--  2.0 unx      971 b- defN 24-Apr-08 20:26 kolibri/backend/pytorch/trainers/plugins/functional/weight_extractor.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-02 15:34 kolibri/backend/pytorch/trainers/plugins/loggers/__init__.py
+-rw-r--r--  2.0 unx     1661 b- defN 24-Apr-08 20:26 kolibri/backend/pytorch/trainers/plugins/loggers/clearml_logger.py
+-rw-r--r--  2.0 unx      817 b- defN 24-Apr-08 20:26 kolibri/backend/pytorch/trainers/plugins/loggers/log_file.py
+-rw-r--r--  2.0 unx     4500 b- defN 24-Apr-08 20:26 kolibri/backend/pytorch/trainers/plugins/loggers/loss_file.py
+-rw-r--r--  2.0 unx     1282 b- defN 24-Apr-08 20:26 kolibri/backend/pytorch/trainers/plugins/loggers/metric_history.py
+-rw-r--r--  2.0 unx     2548 b- defN 24-Apr-08 20:26 kolibri/backend/pytorch/trainers/plugins/loggers/tensorboard.py
+-rw-r--r--  2.0 unx     2542 b- defN 24-Apr-08 20:26 kolibri/backend/pytorch/trainers/plugins/loggers/wandb.py
+-rw-r--r--  2.0 unx      111 b- defN 24-Apr-02 15:34 kolibri/backend/pytorch/visual/__init__.py
+-rw-r--r--  2.0 unx     1910 b- defN 24-Apr-02 15:34 kolibri/backend/pytorch/visual/activations.py
+-rw-r--r--  2.0 unx     3350 b- defN 24-Apr-02 15:34 kolibri/backend/pytorch/visual/manifold.py
+-rw-r--r--  2.0 unx     3133 b- defN 24-Apr-08 20:26 kolibri/backend/pytorch/visual/ner_html.py
+-rw-r--r--  2.0 unx     7528 b- defN 24-Apr-08 15:04 kolibri/backend/pytorch/visual/training_curves.py
+-rw-r--r--  2.0 unx      909 b- defN 24-Apr-08 20:26 kolibri/backend/pytorch/visual/tree_printer.py
+-rw-r--r--  2.0 unx      157 b- defN 24-Apr-06 12:47 kolibri/backend/sklearn/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 12:47 kolibri/backend/sklearn/extensions/__init__.py
+-rw-r--r--  2.0 unx    18744 b- defN 24-Apr-06 12:47 kolibri/backend/sklearn/extensions/decision_tree_log_reg.py
+-rw-r--r--  2.0 unx     1100 b- defN 24-Apr-06 12:47 kolibri/backend/sklearn/extensions/distributed_nn.py
+-rw-r--r--  2.0 unx    15651 b- defN 24-Apr-06 12:47 kolibri/backend/sklearn/extensions/lazy_learner.py
+-rw-r--r--  2.0 unx    14741 b- defN 24-Apr-06 12:47 kolibri/backend/sklearn/extensions/lookup_learner.py
+-rw-r--r--  2.0 unx       65 b- defN 24-Apr-06 12:47 kolibri/backend/sklearn/meta/__init__.py
+-rw-r--r--  2.0 unx    13257 b- defN 24-Apr-06 12:47 kolibri/backend/sklearn/meta/chain_model.py
+-rw-r--r--  2.0 unx    28317 b- defN 24-Apr-06 12:47 kolibri/backend/sklearn/meta/ecoc_model.py
+-rw-r--r--  2.0 unx    28328 b- defN 24-Apr-06 12:47 kolibri/backend/sklearn/meta/ensemble_samplers.py
+-rw-r--r--  2.0 unx     7646 b- defN 24-Apr-06 12:47 kolibri/backend/sklearn/meta/multi_output_estimator.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 12:47 kolibri/backend/sklearn/meta/ecoc/__init__.py
+-rw-r--r--  2.0 unx     8616 b- defN 24-Apr-06 12:47 kolibri/backend/sklearn/meta/ecoc/code_matrix.py
+-rw-r--r--  2.0 unx     5551 b- defN 24-Apr-06 12:47 kolibri/backend/sklearn/meta/ecoc/criterion.py
+-rw-r--r--  2.0 unx     9095 b- defN 24-Apr-06 12:47 kolibri/backend/sklearn/meta/ecoc/decoder.py
+-rw-r--r--  2.0 unx     3869 b- defN 24-Apr-06 12:47 kolibri/backend/sklearn/meta/ecoc/sffs.py
+-rw-r--r--  2.0 unx     2953 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/__init__.py
+-rw-r--r--  2.0 unx      519 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/logger.py
+-rw-r--r--  2.0 unx      308 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/macros.py
+-rw-r--r--  2.0 unx      457 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/autoencoder/__init__.py
+-rw-r--r--  2.0 unx     7029 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/autoencoder/base_autoencoder.py
+-rw-r--r--  2.0 unx     3339 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/autoencoder/conv_autoencoder.py
+-rw-r--r--  2.0 unx     2611 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/autoencoder/deep_autoencoder.py
+-rw-r--r--  2.0 unx     3757 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/autoencoder/variational_autoencoder.py
+-rw-r--r--  2.0 unx      204 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/autoencoder/decoders/__init__.py
+-rw-r--r--  2.0 unx     2091 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/autoencoder/decoders/att_gru_decoder.py
+-rw-r--r--  2.0 unx     1294 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/autoencoder/decoders/gru_decoder.py
+-rw-r--r--  2.0 unx     1213 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/autoencoder/decoders/lstm_decoder.py
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/autoencoder/encoders/__init__.py
+-rw-r--r--  2.0 unx     1257 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/autoencoder/encoders/gru_encoder.py
+-rw-r--r--  2.0 unx     1383 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/autoencoder/encoders/lstm_encoder.py
+-rw-r--r--  2.0 unx      134 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/callbacks/__init__.py
+-rw-r--r--  2.0 unx     2025 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/callbacks/conll_call_back.py
+-rw-r--r--  2.0 unx     2241 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/callbacks/eval_callBack.py
+-rw-r--r--  2.0 unx     4874 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/callbacks/save_callback.py
+-rw-r--r--  2.0 unx      320 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/embeddings/__init__.py
+-rw-r--r--  2.0 unx     1709 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/embeddings/bare_embedding.py
+-rw-r--r--  2.0 unx     4642 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/embeddings/base_embedding.py
+-rw-r--r--  2.0 unx     1322 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/embeddings/bert_embedding.py
+-rw-r--r--  2.0 unx     8420 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/embeddings/elmo_embedding.py
+-rw-r--r--  2.0 unx     3196 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/embeddings/embedding_trainer.py
+-rw-r--r--  2.0 unx     1952 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/embeddings/fasttext_embedding.py
+-rw-r--r--  2.0 unx     2568 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/embeddings/glove_embedding.py
+-rw-r--r--  2.0 unx     9637 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/embeddings/loader.py
+-rw-r--r--  2.0 unx    14296 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/embeddings/loader_albert.py
+-rw-r--r--  2.0 unx     4114 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/embeddings/numeric_feature_embedding.py
+-rw-r--r--  2.0 unx     4911 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/embeddings/stacked_embedding.py
+-rw-r--r--  2.0 unx     3830 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/embeddings/transformer_embedding.py
+-rw-r--r--  2.0 unx     3347 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/embeddings/word_embedding.py
+-rw-r--r--  2.0 unx      679 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/gan/__init__.py
+-rw-r--r--  2.0 unx    15332 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/gan/_transformer.py
+-rw-r--r--  2.0 unx      462 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/gan/bgm.py
+-rw-r--r--  2.0 unx     3406 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/gan/discriminator.py
+-rw-r--r--  2.0 unx     2727 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/gan/generator.py
+-rw-r--r--  2.0 unx      412 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/gan/ohe.py
+-rw-r--r--  2.0 unx     1015 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/layers/__init__.py
+-rw-r--r--  2.0 unx     3258 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/layers/att_wgt_avg_layer.py
+-rw-r--r--  2.0 unx     1528 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/layers/behdanau_attention.py
+-rw-r--r--  2.0 unx     4389 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/layers/conditional_random_field.py
+-rw-r--r--  2.0 unx     1047 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/layers/folding_layer.py
+-rw-r--r--  2.0 unx     4173 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/layers/gen_activation.py
+-rw-r--r--  2.0 unx     2033 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/layers/highway_layer.py
+-rw-r--r--  2.0 unx     3088 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/layers/kmax_pool_layer.py
+-rw-r--r--  2.0 unx     1129 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/layers/layer_utils.py
+-rw-r--r--  2.0 unx     5012 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/layers/multi_head_attention.py
+-rw-r--r--  2.0 unx      787 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/layers/non_masking_layer.py
+-rw-r--r--  2.0 unx     1892 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/layers/residual.py
+-rw-r--r--  2.0 unx      372 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/losses/__init__.py
+-rw-r--r--  2.0 unx     1416 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/losses/conditional_loss.py
+-rw-r--r--  2.0 unx     2959 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/losses/custom_loses.py
+-rw-r--r--  2.0 unx     2299 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/losses/gradient_penalty.py
+-rw-r--r--  2.0 unx      292 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/metrics/__init__.py
+-rw-r--r--  2.0 unx     2525 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/metrics/multi_label_classification.py
+-rw-r--r--  2.0 unx    14331 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/metrics/sequence_labeling.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/tasks/__init__.py
+-rw-r--r--  2.0 unx     5384 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/tasks/base_model.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/tasks/structured/__init__.py
+-rw-r--r--  2.0 unx     7871 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/tasks/structured/base_model.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/tasks/structured/regression/__init__.py
+-rw-r--r--  2.0 unx     4756 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/tasks/structured/regression/base_model.py
+-rw-r--r--  2.0 unx     1802 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/tasks/structured/regression/dnn_regression_estimator.py
+-rw-r--r--  2.0 unx     2744 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/tasks/structured/regression/models.py
+-rw-r--r--  2.0 unx      517 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/tasks/structured/synthetic/__init__.py
+-rw-r--r--  2.0 unx    20393 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/tasks/structured/synthetic/_synthesizer.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/tasks/text/__init__.py
+-rw-r--r--  2.0 unx      417 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/tasks/text/classification/__init__.py
+-rw-r--r--  2.0 unx    15208 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/tasks/text/classification/base_model.py
+-rw-r--r--  2.0 unx     3381 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/tasks/text/classification/cnn_attention_model.py
+-rw-r--r--  2.0 unx     6196 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/tasks/text/classification/dpcnn_model.py
+-rw-r--r--  2.0 unx    28815 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/tasks/text/classification/models.py
+-rw-r--r--  2.0 unx      429 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/tasks/text/labeling/__init__.py
+-rw-r--r--  2.0 unx    17329 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/tasks/text/labeling/base_model.py
+-rw-r--r--  2.0 unx     2846 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/tasks/text/labeling/bi_gru_crf_model.py
+-rw-r--r--  2.0 unx     2249 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/tasks/text/labeling/bi_gru_model.py
+-rw-r--r--  2.0 unx     2991 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/tasks/text/labeling/bi_lstm_crf_model.py
+-rw-r--r--  2.0 unx     2295 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/tasks/text/labeling/bi_lstm_model.py
+-rw-r--r--  2.0 unx     1440 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/tasks/text/labeling/cnn_lstm_model.py
+-rw-r--r--  2.0 unx       84 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/tasks/text/seq2seq/__init__.py
+-rw-r--r--  2.0 unx     2443 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/tasks/text/seq2seq/generator.py
+-rw-r--r--  2.0 unx    13913 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/tasks/text/seq2seq/model.py
+-rw-r--r--  2.0 unx     1158 b- defN 24-Apr-06 13:18 kolibri/backend/tensorflow/utils/__init__.py
+-rw-r--r--  2.0 unx      740 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/utils/_load_demo.py
+-rw-r--r--  2.0 unx      919 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/utils/data.py
+-rw-r--r--  2.0 unx     1629 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/utils/model.py
+-rw-r--r--  2.0 unx      862 b- defN 24-Apr-06 12:47 kolibri/backend/tensorflow/utils/serialize.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 12:47 kolibri/bin/__init__.py
+-rw-r--r--  2.0 unx      471 b- defN 24-Apr-06 12:47 kolibri/bin/datasets_configs.json
+-rw-r--r--  2.0 unx     2731 b- defN 24-Apr-06 12:47 kolibri/bin/kolibri-download.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 12:47 kolibri/callbacks/__init__.py
+-rw-r--r--  2.0 unx      536 b- defN 24-Apr-06 12:47 kolibri/callbacks/base.py
+-rw-r--r--  2.0 unx     3298 b- defN 24-Apr-06 12:47 kolibri/callbacks/callbacks_manager.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 12:47 kolibri/core/__init__.py
+-rw-r--r--  2.0 unx    18812 b- defN 24-Apr-06 12:47 kolibri/core/component.py
+-rw-r--r--  2.0 unx      223 b- defN 24-Apr-06 12:47 kolibri/core/document.py
+-rw-r--r--  2.0 unx     1111 b- defN 24-Apr-06 12:47 kolibri/core/entity.py
+-rw-r--r--  2.0 unx     4052 b- defN 24-Apr-06 12:47 kolibri/core/modules.py
+-rw-r--r--  2.0 unx    17570 b- defN 24-Apr-06 12:47 kolibri/core/pipeline.py
+-rw-r--r--  2.0 unx     2289 b- defN 24-Apr-06 12:47 kolibri/core/serializable.py
+-rw-r--r--  2.0 unx     5771 b- defN 24-Apr-06 12:47 kolibri/core/vocabulary.py
+-rw-r--r--  2.0 unx      117 b- defN 24-Apr-06 12:47 kolibri/data/__init__.py
+-rw-r--r--  2.0 unx     4452 b- defN 24-Apr-06 12:47 kolibri/data/auto_downloader.py
+-rw-r--r--  2.0 unx     2246 b- defN 24-Apr-06 12:47 kolibri/data/base_stream.py
+-rw-r--r--  2.0 unx     4978 b- defN 24-Apr-06 12:47 kolibri/data/blob.py
+-rw-r--r--  2.0 unx    67193 b- defN 24-Apr-08 20:26 kolibri/data/data_base.py
+-rw-r--r--  2.0 unx    29540 b- defN 24-Apr-06 12:47 kolibri/data/dataset.py
+-rw-r--r--  2.0 unx      234 b- defN 24-Apr-06 12:47 kolibri/data/document.py
+-rw-r--r--  2.0 unx    39086 b- defN 24-Apr-06 12:47 kolibri/data/downloader.py
+-rw-r--r--  2.0 unx    10372 b- defN 24-Apr-06 12:47 kolibri/data/file_stream.py
+-rw-r--r--  2.0 unx      534 b- defN 24-Apr-06 12:47 kolibri/data/iterator.py
+-rw-r--r--  2.0 unx      743 b- defN 24-Apr-06 12:47 kolibri/data/resources.py
+-rw-r--r--  2.0 unx    10130 b- defN 24-Apr-06 12:47 kolibri/data/schemes.py
+-rw-r--r--  2.0 unx    42659 b- defN 24-Apr-06 12:47 kolibri/data/settings.py
+-rw-r--r--  2.0 unx     5610 b- defN 24-Apr-06 12:47 kolibri/data/streams.py
+-rw-r--r--  2.0 unx     7910 b- defN 24-Apr-06 12:47 kolibri/data/text.py
+-rw-r--r--  2.0 unx    44023 b- defN 24-Apr-06 13:11 kolibri/data/utils.py
+-rw-r--r--  2.0 unx     3883 b- defN 24-Apr-06 23:18 kolibri/data/datasets/__init__.py
+-rw-r--r--  2.0 unx     9397 b- defN 24-Apr-08 20:26 kolibri/data/datasets/base.py
+-rw-r--r--  2.0 unx    91465 b- defN 24-Apr-06 22:56 kolibri/data/datasets/document_classification.py
+-rw-r--r--  2.0 unx   200111 b- defN 24-Apr-07 19:38 kolibri/data/datasets/sequence_labeling.py
+-rw-r--r--  2.0 unx       94 b- defN 24-Apr-06 12:47 kolibri/data/format/__init__.py
+-rw-r--r--  2.0 unx      539 b- defN 24-Apr-06 12:47 kolibri/data/format/conll.py
+-rw-r--r--  2.0 unx      385 b- defN 24-Apr-06 12:47 kolibri/data/format/csv.py
+-rw-r--r--  2.0 unx      149 b- defN 24-Apr-06 12:47 kolibri/data/loaders/__init__.py
+-rw-r--r--  2.0 unx      960 b- defN 24-Apr-06 12:47 kolibri/data/loaders/arxiv.py
+-rw-r--r--  2.0 unx     2516 b- defN 24-Apr-06 12:47 kolibri/data/loaders/base.py
+-rw-r--r--  2.0 unx     2238 b- defN 24-Apr-06 12:47 kolibri/data/loaders/csv_loader.py
+-rw-r--r--  2.0 unx     4578 b- defN 24-Apr-06 12:47 kolibri/data/loaders/pdf.py
+-rw-r--r--  2.0 unx     1973 b- defN 24-Apr-06 12:47 kolibri/data/loaders/text.py
+-rw-r--r--  2.0 unx     7710 b- defN 24-Apr-06 12:47 kolibri/data/loaders/web_base.py
+-rw-r--r--  2.0 unx      242 b- defN 24-Apr-06 12:47 kolibri/data/parsers/__init__.py
+-rw-r--r--  2.0 unx     1929 b- defN 24-Apr-06 12:47 kolibri/data/parsers/audio.py
+-rw-r--r--  2.0 unx     1090 b- defN 24-Apr-06 12:47 kolibri/data/parsers/base.py
+-rw-r--r--  2.0 unx     2429 b- defN 24-Apr-06 12:47 kolibri/data/parsers/generic.py
+-rw-r--r--  2.0 unx      813 b- defN 24-Apr-06 12:47 kolibri/data/parsers/pdf.py
+-rw-r--r--  2.0 unx      906 b- defN 24-Apr-06 12:47 kolibri/data/parsers/registry.py
+-rw-r--r--  2.0 unx      453 b- defN 24-Apr-06 12:47 kolibri/data/parsers/txt.py
+-rw-r--r--  2.0 unx       85 b- defN 24-Apr-06 12:47 kolibri/data/parsers/html/__init__.py
+-rw-r--r--  2.0 unx     1567 b- defN 24-Apr-06 12:47 kolibri/data/parsers/html/bs4.py
+-rw-r--r--  2.0 unx      929 b- defN 24-Apr-06 12:47 kolibri/data/parsers/html/hyperlinks.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 12:47 kolibri/data/text/__init__.py
+-rw-r--r--  2.0 unx     2246 b- defN 24-Apr-06 12:47 kolibri/data/text/base_stream.py
+-rw-r--r--  2.0 unx     1236 b- defN 24-Apr-06 12:47 kolibri/data/text/corpus.py
+-rw-r--r--  2.0 unx    29550 b- defN 24-Apr-06 12:47 kolibri/data/text/dataset.py
+-rw-r--r--  2.0 unx    10385 b- defN 24-Apr-06 12:47 kolibri/data/text/file_stream.py
+-rw-r--r--  2.0 unx     5145 b- defN 24-Apr-06 12:47 kolibri/data/text/generators.py
+-rw-r--r--  2.0 unx      534 b- defN 24-Apr-06 12:47 kolibri/data/text/iterator.py
+-rw-r--r--  2.0 unx    10130 b- defN 24-Apr-06 12:47 kolibri/data/text/schemes.py
+-rw-r--r--  2.0 unx     5615 b- defN 24-Apr-06 12:47 kolibri/data/text/streams.py
+-rw-r--r--  2.0 unx     7915 b- defN 24-Apr-06 12:47 kolibri/data/text/text.py
+-rw-r--r--  2.0 unx      104 b- defN 24-Apr-06 12:47 kolibri/data/text/format/__init__.py
+-rw-r--r--  2.0 unx      539 b- defN 24-Apr-06 12:47 kolibri/data/text/format/conll.py
+-rw-r--r--  2.0 unx      385 b- defN 24-Apr-06 12:47 kolibri/data/text/format/csv.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 12:47 kolibri/data/text/quality/__init__.py
+-rw-r--r--  2.0 unx     4796 b- defN 24-Apr-06 12:47 kolibri/data/text/quality/cosineSimilarity.py
+-rw-r--r--  2.0 unx      983 b- defN 24-Apr-06 12:47 kolibri/data/text/quality/mismatch.py
+-rw-r--r--  2.0 unx      166 b- defN 24-Apr-06 12:47 kolibri/data/text/quality/pairwise_cos_sim.py
+-rw-r--r--  2.0 unx      837 b- defN 24-Apr-06 12:47 kolibri/data/text/quality/similar.py
+-rw-r--r--  2.0 unx       47 b- defN 24-Apr-06 12:47 kolibri/datasets/__init__.py
+-rw-r--r--  2.0 unx     1800 b- defN 24-Apr-06 12:47 kolibri/datasets/read_data.py
+-rw-r--r--  2.0 unx       61 b- defN 24-Apr-06 12:47 kolibri/datasets/reader/__init__.py
+-rw-r--r--  2.0 unx     3092 b- defN 24-Apr-06 12:47 kolibri/datasets/reader/base_reader.py
+-rw-r--r--  2.0 unx     4055 b- defN 24-Apr-06 12:47 kolibri/datasets/reader/classification.py
+-rw-r--r--  2.0 unx     2213 b- defN 24-Apr-06 12:47 kolibri/datasets/reader/conll.py
+-rw-r--r--  2.0 unx    30779 b- defN 24-Apr-06 12:47 kolibri/datasets/reader/dialogs_reader.py
+-rw-r--r--  2.0 unx     8005 b- defN 24-Apr-06 12:47 kolibri/datasets/reader/dstc2.py
+-rw-r--r--  2.0 unx     4919 b- defN 24-Apr-06 12:47 kolibri/datasets/reader/snips.py
+-rw-r--r--  2.0 unx     3531 b- defN 24-Apr-06 12:47 kolibri/distances/__init__.py
+-rw-r--r--  2.0 unx     4899 b- defN 24-Apr-06 12:47 kolibri/distances/base_categorical.py
+-rw-r--r--  2.0 unx     2551 b- defN 24-Apr-06 12:47 kolibri/distances/eskin.py
+-rw-r--r--  2.0 unx     3907 b- defN 24-Apr-06 12:47 kolibri/distances/goodall.py
+-rw-r--r--  2.0 unx     6368 b- defN 24-Apr-06 12:47 kolibri/distances/heom.py
+-rw-r--r--  2.0 unx     5015 b- defN 24-Apr-06 12:47 kolibri/distances/hvdm.py
+-rw-r--r--  2.0 unx     1226 b- defN 24-Apr-06 12:47 kolibri/distances/lin.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 12:47 kolibri/evaluation/__init__.py
+-rw-r--r--  2.0 unx     7911 b- defN 24-Apr-06 12:47 kolibri/evaluation/classifier_evaluator.py
+-rw-r--r--  2.0 unx     2489 b- defN 24-Apr-06 12:47 kolibri/evaluation/clustering_evaluator.py
+-rw-r--r--  2.0 unx    41666 b- defN 24-Apr-06 12:47 kolibri/evaluation/model_plot.py
+-rw-r--r--  2.0 unx      809 b- defN 24-Apr-06 12:47 kolibri/evaluation/metrics/__init__.py
+-rw-r--r--  2.0 unx     5578 b- defN 24-Apr-06 12:47 kolibri/evaluation/metrics/anomaly.py
+-rw-r--r--  2.0 unx     1792 b- defN 24-Apr-06 12:47 kolibri/evaluation/metrics/base_metric.py
+-rw-r--r--  2.0 unx     9438 b- defN 24-Apr-06 12:47 kolibri/evaluation/metrics/classification.py
+-rw-r--r--  2.0 unx     7198 b- defN 24-Apr-06 12:47 kolibri/evaluation/metrics/clustering.py
+-rw-r--r--  2.0 unx     8757 b- defN 24-Apr-06 12:47 kolibri/evaluation/metrics/metric_utils.py
+-rw-r--r--  2.0 unx     9491 b- defN 24-Apr-06 12:47 kolibri/evaluation/metrics/regression.py
+-rw-r--r--  2.0 unx    10235 b- defN 24-Apr-06 12:47 kolibri/evaluation/metrics/time_series.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 12:47 kolibri/evaluators/__init__.py
+-rw-r--r--  2.0 unx     8796 b- defN 24-Apr-06 12:47 kolibri/evaluators/classifier_evaluator.py
+-rw-r--r--  2.0 unx     2489 b- defN 24-Apr-06 12:47 kolibri/evaluators/clustering_evaluator.py
+-rw-r--r--  2.0 unx    41682 b- defN 24-Apr-06 12:47 kolibri/evaluators/model_plot.py
+-rw-r--r--  2.0 unx     3215 b- defN 24-Apr-06 12:47 kolibri/evaluators/synthetic_data.py
+-rw-r--r--  2.0 unx      224 b- defN 24-Apr-06 12:47 kolibri/experiment_tracking/__init__.py
+-rw-r--r--  2.0 unx     6170 b- defN 24-Apr-06 12:47 kolibri/experiment_tracking/experiment_logger.py
+-rw-r--r--  2.0 unx     4971 b- defN 24-Apr-06 12:47 kolibri/experiment_tracking/mlflow_logger.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 12:47 kolibri/explainers/__init__.py
+-rw-r--r--  2.0 unx    12089 b- defN 24-Apr-06 12:47 kolibri/explainers/shap_explainer.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 12:47 kolibri/features/__init__.py
+-rw-r--r--  2.0 unx     2781 b- defN 24-Apr-06 12:47 kolibri/features/base_feature.py
+-rw-r--r--  2.0 unx     1431 b- defN 24-Apr-06 12:47 kolibri/features/basefeaturizer.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 12:47 kolibri/features/tabular/__init__.py
+-rw-r--r--  2.0 unx     1763 b- defN 24-Apr-06 12:47 kolibri/features/tabular/time_serie_featurizer.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 12:47 kolibri/features/text/__init__.py
+-rw-r--r--  2.0 unx     8352 b- defN 24-Apr-06 12:47 kolibri/features/text/feature_functions.py
+-rw-r--r--  2.0 unx    10000 b- defN 24-Apr-06 12:47 kolibri/features/text/hashing_tfidf_vectorizer.py
+-rw-r--r--  2.0 unx     5801 b- defN 24-Apr-06 12:47 kolibri/features/text/text_features.py
+-rw-r--r--  2.0 unx     6336 b- defN 24-Apr-06 12:47 kolibri/features/text/tf_idf_featurizer.py
+-rw-r--r--  2.0 unx     5853 b- defN 24-Apr-06 12:47 kolibri/features/text/tf_idf_topics_vectorizer.py
+-rw-r--r--  2.0 unx     8121 b- defN 24-Apr-06 12:47 kolibri/features/text/tfidf_weighted_embedder.py
+-rw-r--r--  2.0 unx      346 b- defN 24-Apr-06 12:47 kolibri/features/text/embedders/__init__.py
+-rw-r--r--  2.0 unx     3700 b- defN 24-Apr-06 11:12 kolibri/features/text/embedders/abstract_embedder.py
+-rw-r--r--  2.0 unx     3709 b- defN 24-Apr-06 12:47 kolibri/features/text/embedders/base.py
+-rw-r--r--  2.0 unx     1347 b- defN 24-Apr-06 12:47 kolibri/features/text/embedders/bow_embedder.py
+-rw-r--r--  2.0 unx     9928 b- defN 24-Apr-06 12:47 kolibri/features/text/embedders/elmo_embedder.py
+-rw-r--r--  2.0 unx     1568 b- defN 24-Apr-06 12:47 kolibri/features/text/embedders/fasttext_embedder.py
+-rw-r--r--  2.0 unx     2027 b- defN 24-Apr-06 12:47 kolibri/features/text/embedders/glove_embedder.py
+-rw-r--r--  2.0 unx     4096 b- defN 24-Apr-06 12:47 kolibri/features/text/embedders/llamacpp.py
+-rw-r--r--  2.0 unx    17705 b- defN 24-Apr-06 12:47 kolibri/features/text/embedders/openai.py
+-rw-r--r--  2.0 unx     2466 b- defN 24-Apr-06 12:47 kolibri/features/text/embedders/tensorflow_hub.py
+-rw-r--r--  2.0 unx     4920 b- defN 24-Apr-06 11:12 kolibri/features/text/embedders/transformers_embedder.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 12:47 kolibri/features/timeseries/__init__.py
+-rw-r--r--  2.0 unx    31971 b- defN 24-Apr-06 12:47 kolibri/features/timeseries/features_utils.py
+-rw-r--r--  2.0 unx    10656 b- defN 24-Apr-06 12:47 kolibri/features/timeseries/ts_featurizer.py
+-rw-r--r--  2.0 unx     7659 b- defN 24-Apr-06 12:47 kolibri/features/timeseries/utils.py
+-rw-r--r--  2.0 unx      358 b- defN 24-Apr-06 12:47 kolibri/features/timeseries/feature_extraction/__init__.py
+-rw-r--r--  2.0 unx    16661 b- defN 24-Apr-06 12:47 kolibri/features/timeseries/feature_extraction/data.py
+-rw-r--r--  2.0 unx    13772 b- defN 24-Apr-06 12:47 kolibri/features/timeseries/feature_extraction/extraction.py
+-rw-r--r--  2.0 unx    81555 b- defN 24-Apr-06 12:47 kolibri/features/timeseries/feature_extraction/feature_calculators.py
+-rw-r--r--  2.0 unx    14105 b- defN 24-Apr-06 12:47 kolibri/features/timeseries/feature_extraction/settings.py
+-rw-r--r--  2.0 unx      606 b- defN 24-Apr-06 12:47 kolibri/features/timeseries/feature_selection/__init__.py
+-rw-r--r--  2.0 unx    15671 b- defN 24-Apr-06 12:47 kolibri/features/timeseries/feature_selection/relevance.py
+-rw-r--r--  2.0 unx     7871 b- defN 24-Apr-06 12:47 kolibri/features/timeseries/feature_selection/selection.py
+-rw-r--r--  2.0 unx     8691 b- defN 24-Apr-06 12:47 kolibri/features/timeseries/feature_selection/significance_tests.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 12:47 kolibri/formers/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 12:47 kolibri/formers/tabular/__init__.py
+-rw-r--r--  2.0 unx     1043 b- defN 24-Apr-06 12:47 kolibri/formers/tabular/clustering.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 12:47 kolibri/formers/text/__init__.py
+-rw-r--r--  2.0 unx     4315 b- defN 24-Apr-06 12:47 kolibri/formers/text/classifier.py
+-rw-r--r--  2.0 unx      230 b- defN 24-Apr-06 12:47 kolibri/formers/text/sentiment.py
+-rw-r--r--  2.0 unx     4515 b- defN 24-Apr-06 12:47 kolibri/formers/text/similarity.py
+-rw-r--r--  2.0 unx    40754 b- defN 24-Apr-06 12:47 kolibri/formers/text/topic_former.py
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-06 12:47 kolibri/indexers/__init__.py
+-rw-r--r--  2.0 unx     2657 b- defN 24-Apr-06 12:47 kolibri/indexers/base_indexer.py
+-rw-r--r--  2.0 unx     1239 b- defN 24-Apr-06 12:47 kolibri/indexers/kolibri_label_encoder.py
+-rw-r--r--  2.0 unx     3482 b- defN 24-Apr-06 13:18 kolibri/indexers/label_indexer.py
+-rw-r--r--  2.0 unx     1248 b- defN 24-Apr-06 12:47 kolibri/indexers/multi_content_indexer.py
+-rw-r--r--  2.0 unx     1131 b- defN 24-Apr-06 12:47 kolibri/indexers/multi_label.py
+-rw-r--r--  2.0 unx     2394 b- defN 24-Apr-06 12:47 kolibri/indexers/multi_target_indexer.py
+-rw-r--r--  2.0 unx     4944 b- defN 24-Apr-06 12:47 kolibri/indexers/sequence_char_indexer.py
+-rw-r--r--  2.0 unx     6012 b- defN 24-Apr-06 12:47 kolibri/indexers/sequence_indexer.py
+-rw-r--r--  2.0 unx     5940 b- defN 24-Apr-06 12:47 kolibri/indexers/text_indexer.py
+-rw-r--r--  2.0 unx       43 b- defN 24-Apr-06 12:47 kolibri/knowledge/__init__.py
+-rw-r--r--  2.0 unx     1173 b- defN 24-Apr-06 12:47 kolibri/knowledge/domain.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 12:47 kolibri/llms/__init__.py
+-rw-r--r--  2.0 unx     5183 b- defN 24-Apr-06 12:47 kolibri/llms/base.py
+-rw-r--r--  2.0 unx    25099 b- defN 24-Apr-06 12:47 kolibri/llms/openai.py
+-rw-r--r--  2.0 unx    11163 b- defN 24-Apr-06 12:47 kolibri/mlflow/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 12:47 kolibri/optimizers/__init__.py
+-rw-r--r--  2.0 unx     9226 b- defN 24-Apr-06 12:47 kolibri/optimizers/metric.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 12:47 kolibri/optimizers/optuna/__init__.py
+-rw-r--r--  2.0 unx    10868 b- defN 24-Apr-06 12:47 kolibri/optimizers/optuna/objective.py
+-rw-r--r--  2.0 unx     2889 b- defN 24-Apr-06 12:47 kolibri/optimizers/optuna/tuner.py
+-rw-r--r--  2.0 unx       49 b- defN 24-Apr-06 12:47 kolibri/output/__init__.py
+-rw-r--r--  2.0 unx     3303 b- defN 24-Apr-06 12:47 kolibri/output/display.py
+-rw-r--r--  2.0 unx     5694 b- defN 24-Apr-06 12:47 kolibri/output/display_backend.py
+-rw-r--r--  2.0 unx     1637 b- defN 24-Apr-06 12:47 kolibri/output/display_component.py
+-rw-r--r--  2.0 unx     4514 b- defN 24-Apr-06 12:47 kolibri/output/progress_bar.py
+-rw-r--r--  2.0 unx       40 b- defN 24-Apr-06 12:47 kolibri/preprocess/__init__.py
+-rw-r--r--  2.0 unx    13211 b- defN 24-Apr-06 12:47 kolibri/preprocess/tabular/DataFrameVectorizer.py
+-rw-r--r--  2.0 unx     1780 b- defN 24-Apr-06 12:47 kolibri/preprocess/tabular/__init__.py
+-rw-r--r--  2.0 unx     3030 b- defN 24-Apr-06 12:47 kolibri/preprocess/tabular/binning.py
+-rw-r--r--  2.0 unx     8728 b- defN 24-Apr-06 12:47 kolibri/preprocess/tabular/boruta_py.py
+-rw-r--r--  2.0 unx     1837 b- defN 24-Apr-06 12:47 kolibri/preprocess/tabular/category_transformer.py
+-rw-r--r--  2.0 unx     5219 b- defN 24-Apr-06 12:47 kolibri/preprocess/tabular/cluster.py
+-rw-r--r--  2.0 unx      783 b- defN 24-Apr-06 12:47 kolibri/preprocess/tabular/columns_remover.py
+-rw-r--r--  2.0 unx     1556 b- defN 24-Apr-06 12:47 kolibri/preprocess/tabular/columns_transfromer.py
+-rw-r--r--  2.0 unx    11658 b- defN 24-Apr-06 12:47 kolibri/preprocess/tabular/data_imputer.py
+-rw-r--r--  2.0 unx     2970 b- defN 24-Apr-06 12:47 kolibri/preprocess/tabular/dummy_converter.py
+-rw-r--r--  2.0 unx    13500 b- defN 24-Apr-06 12:47 kolibri/preprocess/tabular/feature_interaction.py
+-rw-r--r--  2.0 unx    10314 b- defN 24-Apr-06 12:47 kolibri/preprocess/tabular/feature_selection.py
+-rw-r--r--  2.0 unx     4401 b- defN 24-Apr-06 12:47 kolibri/preprocess/tabular/infer_datatype.py
+-rw-r--r--  2.0 unx    13584 b- defN 24-Apr-06 12:47 kolibri/preprocess/tabular/multicollinearity.py
+-rw-r--r--  2.0 unx     4341 b- defN 24-Apr-06 12:47 kolibri/preprocess/tabular/normalize.py
+-rw-r--r--  2.0 unx     2494 b- defN 24-Apr-06 12:47 kolibri/preprocess/tabular/one_hot_encoder_multi.py
+-rw-r--r--  2.0 unx     1620 b- defN 24-Apr-06 12:47 kolibri/preprocess/tabular/ordinal_transformer.py
+-rw-r--r--  2.0 unx     2616 b- defN 24-Apr-06 12:47 kolibri/preprocess/tabular/outlier_remover.py
+-rw-r--r--  2.0 unx   149882 b- defN 24-Apr-06 12:47 kolibri/preprocess/tabular/preprocess.py
+-rw-r--r--  2.0 unx    20056 b- defN 24-Apr-06 12:47 kolibri/preprocess/tabular/preprocessing_pipeline.py
+-rw-r--r--  2.0 unx     3454 b- defN 24-Apr-06 12:47 kolibri/preprocess/tabular/rare_levels.py
+-rw-r--r--  2.0 unx     8598 b- defN 24-Apr-06 12:47 kolibri/preprocess/tabular/reduce_cardinality.py
+-rw-r--r--  2.0 unx     4848 b- defN 24-Apr-06 12:47 kolibri/preprocess/tabular/reduce_dimensionality.py
+-rw-r--r--  2.0 unx     1801 b- defN 24-Apr-06 12:47 kolibri/preprocess/tabular/regression_target_transformer.py
+-rw-r--r--  2.0 unx     2003 b- defN 24-Apr-06 12:47 kolibri/preprocess/tabular/similar_features.py
+-rw-r--r--  2.0 unx     4003 b- defN 24-Apr-06 12:47 kolibri/preprocess/tabular/time_features_extractor.py
+-rw-r--r--  2.0 unx     1808 b- defN 24-Apr-06 12:47 kolibri/preprocess/tabular/univar_outliers.py
+-rw-r--r--  2.0 unx     3531 b- defN 24-Apr-06 12:47 kolibri/preprocess/tabular/zero_variance_remover.py
+-rw-r--r--  2.0 unx       76 b- defN 24-Apr-06 12:47 kolibri/preprocess/text/__init__.py
+-rw-r--r--  2.0 unx     4058 b- defN 24-Apr-06 12:47 kolibri/preprocess/text/capitalization.py
+-rw-r--r--  2.0 unx      596 b- defN 24-Apr-06 12:47 kolibri/preprocess/text/char_splitter.py
+-rw-r--r--  2.0 unx     4297 b- defN 24-Apr-06 12:47 kolibri/preprocess/text/collocation_analyzer.py
+-rw-r--r--  2.0 unx     1412 b- defN 24-Apr-06 12:47 kolibri/preprocess/text/context_builder.py
+-rw-r--r--  2.0 unx     3356 b- defN 24-Apr-06 12:47 kolibri/preprocess/text/dirty_comments_preprocessor.py
+-rw-r--r--  2.0 unx     5305 b- defN 24-Apr-06 12:47 kolibri/preprocess/text/doc_chuncker.py
+-rw-r--r--  2.0 unx     1183 b- defN 24-Apr-06 12:47 kolibri/preprocess/text/mask.py
+-rw-r--r--  2.0 unx     7307 b- defN 24-Apr-06 12:47 kolibri/preprocess/text/ner_preprocessor.py
+-rw-r--r--  2.0 unx     1229 b- defN 24-Apr-06 12:47 kolibri/preprocess/text/random_embeddings_matrix.py
+-rw-r--r--  2.0 unx    10274 b- defN 24-Apr-06 12:47 kolibri/preprocess/text/re_preprocessor.py
+-rw-r--r--  2.0 unx     5800 b- defN 24-Apr-06 12:47 kolibri/preprocess/text/siamese_preprocessor.py
+-rw-r--r--  2.0 unx     1883 b- defN 24-Apr-06 12:47 kolibri/preprocess/text/str_token_reverser.py
+-rw-r--r--  2.0 unx     7566 b- defN 24-Apr-06 12:47 kolibri/preprocess/text/str_utf8_encoder.py
+-rw-r--r--  2.0 unx     6299 b- defN 24-Apr-06 12:47 kolibri/preprocess/text/text_splitter.py
+-rw-r--r--  2.0 unx     2657 b- defN 24-Apr-06 12:47 kolibri/preprocess/text/transformers_preprocessor.py
+-rw-r--r--  2.0 unx     5288 b- defN 24-Apr-06 12:47 kolibri/preprocess/text/cleaning/__email_configs.py
+-rw-r--r--  2.0 unx       67 b- defN 24-Apr-06 12:47 kolibri/preprocess/text/cleaning/__init__.py
+-rw-r--r--  2.0 unx     4348 b- defN 24-Apr-06 12:47 kolibri/preprocess/text/cleaning/cleaning_scripts.py
+-rw-r--r--  2.0 unx    23554 b- defN 24-Apr-06 12:47 kolibri/preprocess/text/cleaning/email2text.py
+-rw-r--r--  2.0 unx     1764 b- defN 24-Apr-06 12:47 kolibri/preprocess/text/cleaning/email_cleaner.py
+-rw-r--r--  2.0 unx     1425 b- defN 24-Apr-06 12:47 kolibri/preprocess/text/cleaning/email_parser.py
+-rw-r--r--  2.0 unx     3279 b- defN 24-Apr-06 12:47 kolibri/preprocess/text/cleaning/header_parser.py
+-rw-r--r--  2.0 unx       82 b- defN 24-Apr-06 12:47 kolibri/preprocess/text/language_detection/__init__.py
+-rw-r--r--  2.0 unx     1420 b- defN 24-Apr-06 12:47 kolibri/preprocess/text/language_detection/lang_detect.py
+-rw-r--r--  2.0 unx     7047 b- defN 24-Apr-06 12:47 kolibri/preprocess/text/translation/Translate_.py
+-rw-r--r--  2.0 unx     1079 b- defN 24-Apr-06 12:47 kolibri/preprocess/text/translation/__init__.py
+-rw-r--r--  2.0 unx     9890 b- defN 24-Apr-06 12:47 kolibri/preprocess/text/translation/client.py
+-rw-r--r--  2.0 unx     9746 b- defN 24-Apr-06 12:47 kolibri/preprocess/text/translation/constants.py
+-rw-r--r--  2.0 unx     1601 b- defN 24-Apr-06 12:47 kolibri/preprocess/text/translation/models.py
+-rw-r--r--  2.0 unx     6090 b- defN 24-Apr-06 12:47 kolibri/preprocess/text/translation/translate.py
+-rw-r--r--  2.0 unx     2640 b- defN 24-Apr-06 12:47 kolibri/preprocess/text/translation/utils.py
+-rw-r--r--  2.0 unx       65 b- defN 24-Apr-06 12:47 kolibri/preprocess/timeseries/__init__.py
+-rw-r--r--  2.0 unx    16072 b- defN 24-Apr-06 12:47 kolibri/preprocess/timeseries/multi_window_generator.py
+-rw-r--r--  2.0 unx    15304 b- defN 24-Apr-06 12:47 kolibri/preprocess/timeseries/multi_window_generator_back.py
+-rw-r--r--  2.0 unx     7919 b- defN 24-Apr-06 12:47 kolibri/preprocess/timeseries/time_series_from_array.py
+-rw-r--r--  2.0 unx     8504 b- defN 24-Apr-06 12:47 kolibri/preprocess/timeseries/window.py
+-rw-r--r--  2.0 unx     7843 b- defN 24-Apr-06 12:47 kolibri/preprocess/timeseries/window_generator.py
+-rw-r--r--  2.0 unx     2131 b- defN 24-Apr-06 12:47 kolibri/samplers/__init__.py
+-rw-r--r--  2.0 unx     5095 b- defN 24-Apr-06 12:47 kolibri/samplers/auto_smpler.py
+-rw-r--r--  2.0 unx     5952 b- defN 24-Apr-06 12:47 kolibri/samplers/conditional.py
+-rw-r--r--  2.0 unx     2651 b- defN 24-Apr-06 12:47 kolibri/samplers/data_sampler.py
+-rw-r--r--  2.0 unx     7780 b- defN 24-Apr-06 12:47 kolibri/samplers/smoteR.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 12:47 kolibri/scripts/__init__.py
+-rw-r--r--  2.0 unx      988 b- defN 24-Apr-06 12:47 kolibri/scripts/check_requirements.py
+-rw-r--r--  2.0 unx     1284 b- defN 24-Apr-06 12:47 kolibri/scripts/install_plugin_deps.py
+-rw-r--r--  2.0 unx       52 b- defN 24-Apr-06 12:47 kolibri/stopwords/__init__.py
+-rw-r--r--  2.0 unx     2016 b- defN 24-Apr-06 12:47 kolibri/stopwords/stp_wrd.py
+-rw-r--r--  2.0 unx      717 b- defN 24-Apr-06 12:47 kolibri/synthetic_data/__init__.py
+-rw-r--r--  2.0 unx     3060 b- defN 24-Apr-06 12:47 kolibri/synthetic_data/anonymization.py
+-rw-r--r--  2.0 unx    45790 b- defN 24-Apr-06 12:47 kolibri/synthetic_data/base.py
+-rw-r--r--  2.0 unx    18063 b- defN 24-Apr-06 12:47 kolibri/synthetic_data/base_contraint.py
+-rw-r--r--  2.0 unx    11107 b- defN 24-Apr-06 12:47 kolibri/synthetic_data/copulagan.py
+-rw-r--r--  2.0 unx    14946 b- defN 24-Apr-06 12:47 kolibri/synthetic_data/copulas.py
+-rw-r--r--  2.0 unx     5656 b- defN 24-Apr-06 12:47 kolibri/synthetic_data/ctgan_synthesizer.py
+-rw-r--r--  2.0 unx    35479 b- defN 24-Apr-06 12:47 kolibri/synthetic_data/data_processor.py
+-rw-r--r--  2.0 unx    21083 b- defN 24-Apr-06 12:47 kolibri/synthetic_data/metadata.py
+-rw-r--r--  2.0 unx     7180 b- defN 24-Apr-06 12:47 kolibri/synthetic_data/single_table.py
+-rw-r--r--  2.0 unx     7177 b- defN 24-Apr-06 12:47 kolibri/synthetic_data/synthcity_lib.py
+-rw-r--r--  2.0 unx     3227 b- defN 24-Apr-06 12:47 kolibri/synthetic_data/synthpop.py
+-rw-r--r--  2.0 unx    10163 b- defN 24-Apr-06 12:47 kolibri/synthetic_data/utils.py
+-rw-r--r--  2.0 unx     1186 b- defN 24-Apr-06 12:47 kolibri/synthetic_data/benchmark/__init__.py
+-rw-r--r--  2.0 unx    15188 b- defN 24-Apr-06 12:47 kolibri/synthetic_data/benchmark/benchmark.py
+-rw-r--r--  2.0 unx     6638 b- defN 24-Apr-06 12:47 kolibri/synthetic_data/benchmark/data.py
+-rw-r--r--  2.0 unx     3309 b- defN 24-Apr-06 12:47 kolibri/synthetic_data/benchmark/metrics.py
+-rw-r--r--  2.0 unx     2241 b- defN 24-Apr-06 12:47 kolibri/synthetic_data/benchmark/ml.py
+-rw-r--r--  2.0 unx     2051 b- defN 24-Apr-06 12:47 kolibri/synthetic_data/benchmark/privacy.py
+-rw-r--r--  2.0 unx     6132 b- defN 24-Apr-06 12:47 kolibri/synthetic_data/benchmark/reporting.py
+-rw-r--r--  2.0 unx     2239 b- defN 24-Apr-06 12:47 kolibri/synthetic_data/benchmark/utility.py
+-rw-r--r--  2.0 unx     5464 b- defN 24-Apr-06 12:47 kolibri/synthetic_data/benchmark/utils.py
+-rw-r--r--  2.0 unx     1063 b- defN 24-Apr-06 12:47 kolibri/synthetic_data/benchmark/synthesizers/__init__.py
+-rw-r--r--  2.0 unx     2022 b- defN 24-Apr-06 12:47 kolibri/synthetic_data/benchmark/synthesizers/base.py
+-rw-r--r--  2.0 unx     7232 b- defN 24-Apr-06 12:47 kolibri/synthetic_data/benchmark/synthesizers/generate.py
+-rw-r--r--  2.0 unx     1337 b- defN 24-Apr-06 12:47 kolibri/synthetic_data/benchmark/synthesizers/identity.py
+-rw-r--r--  2.0 unx     2114 b- defN 24-Apr-06 12:47 kolibri/synthetic_data/benchmark/synthesizers/independent.py
+-rw-r--r--  2.0 unx     5641 b- defN 24-Apr-06 12:47 kolibri/synthetic_data/benchmark/synthesizers/sd.py
+-rw-r--r--  2.0 unx     1665 b- defN 24-Apr-06 12:47 kolibri/synthetic_data/benchmark/synthesizers/uniform.py
+-rw-r--r--  2.0 unx       67 b- defN 24-Apr-06 12:47 kolibri/task/__init__.py
+-rw-r--r--  2.0 unx     7765 b- defN 24-Apr-06 12:47 kolibri/task/dnn_estimator.py
+-rw-r--r--  2.0 unx      104 b- defN 24-Apr-06 12:47 kolibri/task/audio/__init__.py
+-rw-r--r--  2.0 unx     9853 b- defN 24-Apr-06 12:47 kolibri/task/audio/base_model.py
+-rw-r--r--  2.0 unx       75 b- defN 24-Apr-06 12:47 kolibri/task/audio/classification/__init__.py
+-rw-r--r--  2.0 unx     3231 b- defN 24-Apr-06 12:47 kolibri/task/audio/classification/dnn_audio_estimator.py
+-rw-r--r--  2.0 unx    10451 b- defN 24-Apr-06 12:47 kolibri/task/audio/classification/models.py
+-rw-r--r--  2.0 unx      156 b- defN 24-Apr-06 12:47 kolibri/task/tabular/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 12:47 kolibri/task/tabular/anomaly/__init__.py
+-rw-r--r--  2.0 unx     1437 b- defN 24-Apr-06 12:47 kolibri/task/tabular/anomaly/anomaly_estimator.py
+-rw-r--r--  2.0 unx    18943 b- defN 24-Apr-06 12:47 kolibri/task/tabular/anomaly/half_space_trees.py
+-rw-r--r--  2.0 unx      700 b- defN 24-Apr-06 12:47 kolibri/task/tabular/anomaly/models.py
+-rw-r--r--  2.0 unx      742 b- defN 24-Apr-06 12:47 kolibri/task/tabular/anomaly/one_class_anomaly_dector.py
+-rw-r--r--  2.0 unx     3274 b- defN 24-Apr-06 12:47 kolibri/task/tabular/anomaly/semi_supervised_anomaly_dector.py
+-rw-r--r--  2.0 unx     4617 b- defN 24-Apr-06 12:47 kolibri/task/tabular/anomaly/unsupervised_anomaly_dector.py
+-rw-r--r--  2.0 unx       74 b- defN 24-Apr-06 12:47 kolibri/task/tabular/clustering/__init__.py
+-rw-r--r--  2.0 unx     4518 b- defN 24-Apr-06 12:47 kolibri/task/tabular/clustering/clustering.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 12:47 kolibri/task/tabular/regression/__init__.py
+-rw-r--r--  2.0 unx     1748 b- defN 24-Apr-06 12:47 kolibri/task/tabular/regression/dnn_regression_estimator.py
+-rw-r--r--  2.0 unx     2171 b- defN 24-Apr-06 12:47 kolibri/task/tabular/regression/sklearn_regression_estimator.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 12:47 kolibri/task/tabular/rulemining/__init__.py
+-rw-r--r--  2.0 unx     9912 b- defN 24-Apr-06 12:47 kolibri/task/tabular/rulemining/association_rules.py
+-rw-r--r--  2.0 unx      140 b- defN 24-Apr-06 12:47 kolibri/task/text/__init__.py
+-rw-r--r--  2.0 unx      190 b- defN 24-Apr-06 12:47 kolibri/task/text/classification/__init__.py
+-rw-r--r--  2.0 unx     4316 b- defN 24-Apr-06 12:47 kolibri/task/text/classification/dnn_classification_estimator.py
+-rw-r--r--  2.0 unx     3199 b- defN 24-Apr-06 12:47 kolibri/task/text/classification/sklearn_classification_estimator.py
+-rw-r--r--  2.0 unx     3262 b- defN 24-Apr-06 13:12 kolibri/task/text/classification/sklearn_estimator.py
+-rw-r--r--  2.0 unx     3145 b- defN 24-Apr-06 12:47 kolibri/task/text/entities/__init__.py
+-rw-r--r--  2.0 unx     1990 b- defN 24-Apr-06 12:47 kolibri/task/text/entities/common_reg_extractor.py
+-rw-r--r--  2.0 unx    17418 b- defN 24-Apr-06 12:47 kolibri/task/text/entities/crf_entity_extractor.py
+-rw-r--r--  2.0 unx      949 b- defN 24-Apr-06 12:47 kolibri/task/text/entities/dictionaryExtractor.py
+-rw-r--r--  2.0 unx     1111 b- defN 24-Apr-06 12:47 kolibri/task/text/entities/entity.py
+-rw-r--r--  2.0 unx     3007 b- defN 24-Apr-06 12:47 kolibri/task/text/entities/entity_extractor.py
+-rw-r--r--  2.0 unx     4171 b- defN 24-Apr-06 12:47 kolibri/task/text/entities/entity_synonyms.py
+-rw-r--r--  2.0 unx     6339 b- defN 24-Apr-06 12:47 kolibri/task/text/entities/lstm_entity_extractor.py
+-rw-r--r--  2.0 unx     3633 b- defN 24-Apr-06 12:47 kolibri/task/text/entities/person_extractor.py
+-rw-r--r--  2.0 unx     2279 b- defN 24-Apr-06 12:47 kolibri/task/text/entities/preprocessing.py
+-rw-r--r--  2.0 unx     2668 b- defN 24-Apr-06 12:47 kolibri/task/text/entities/regex_extractor.py
+-rw-r--r--  2.0 unx     6945 b- defN 24-Apr-06 12:47 kolibri/task/text/entities/templated_extractor.py
+-rw-r--r--  2.0 unx     3498 b- defN 24-Apr-06 12:47 kolibri/task/text/entities/test.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 12:47 kolibri/task/text/entities_back/__init__.py
+-rw-r--r--  2.0 unx     6458 b- defN 24-Apr-06 12:47 kolibri/task/text/entities_back/common_reg_extractor.py
+-rw-r--r--  2.0 unx    18309 b- defN 24-Apr-06 12:47 kolibri/task/text/entities_back/crf_entity_extractor.py
+-rw-r--r--  2.0 unx     1011 b- defN 24-Apr-06 12:47 kolibri/task/text/entities_back/dictionaryExtractor.py
+-rw-r--r--  2.0 unx     2997 b- defN 24-Apr-06 12:47 kolibri/task/text/entities_back/entity_extractor.py
+-rw-r--r--  2.0 unx     4343 b- defN 24-Apr-06 12:47 kolibri/task/text/entities_back/entity_synonyms.py
+-rw-r--r--  2.0 unx     3188 b- defN 24-Apr-06 12:47 kolibri/task/text/entities_back/person_extractor.py
+-rw-r--r--  2.0 unx     2295 b- defN 24-Apr-06 12:47 kolibri/task/text/entities_back/preprocessing.py
+-rw-r--r--  2.0 unx     2644 b- defN 24-Apr-06 12:47 kolibri/task/text/entities_back/regex_extractor.py
+-rw-r--r--  2.0 unx     6419 b- defN 24-Apr-06 12:47 kolibri/task/text/entities_back/templated_extractor.py
+-rw-r--r--  2.0 unx        5 b- defN 24-Apr-06 12:47 kolibri/task/text/intents/__init__.py
+-rw-r--r--  2.0 unx    10289 b- defN 24-Apr-06 12:47 kolibri/task/text/intents/intent_catcher.py
+-rw-r--r--  2.0 unx     3811 b- defN 24-Apr-06 12:47 kolibri/task/text/intents/intent_expressions.py
+-rw-r--r--  2.0 unx     1437 b- defN 24-Apr-06 12:47 kolibri/task/text/intents/domains/__init__.py
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-06 12:47 kolibri/task/text/sentiment/__init__.py
+-rw-r--r--  2.0 unx    12971 b- defN 24-Apr-06 12:47 kolibri/task/text/sentiment/lexicon_sentiment.py
+-rw-r--r--  2.0 unx    32780 b- defN 24-Apr-06 12:47 kolibri/task/text/sentiment/util.py
+-rw-r--r--  2.0 unx    22769 b- defN 24-Apr-06 12:47 kolibri/task/text/sentiment/vader.py
+-rw-r--r--  2.0 unx     2587 b- defN 24-Apr-06 12:47 kolibri/task/text/similarity/__init__.py
+-rw-r--r--  2.0 unx      559 b- defN 24-Apr-06 12:47 kolibri/task/text/similarity/arxiv.py
+-rw-r--r--  2.0 unx     6717 b- defN 24-Apr-06 12:47 kolibri/task/text/similarity/docarray.py
+-rw-r--r--  2.0 unx     2361 b- defN 24-Apr-06 12:47 kolibri/task/text/similarity/knn.py
+-rw-r--r--  2.0 unx     2907 b- defN 24-Apr-06 12:47 kolibri/task/text/similarity/llama_index.py
+-rw-r--r--  2.0 unx     2907 b- defN 24-Apr-06 12:47 kolibri/task/text/similarity/merger_retriever.py
+-rw-r--r--  2.0 unx      569 b- defN 24-Apr-06 12:47 kolibri/task/text/similarity/pupmed.py
+-rw-r--r--  2.0 unx     2953 b- defN 24-Apr-06 12:47 kolibri/task/text/similarity/svm.py
+-rw-r--r--  2.0 unx     2470 b- defN 24-Apr-06 12:47 kolibri/task/text/similarity/tfidf.py
+-rw-r--r--  2.0 unx      579 b- defN 24-Apr-06 12:47 kolibri/task/text/similarity/wikipedia.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 12:47 kolibri/task/text/spelling/__init__.py
+-rw-r--r--  2.0 unx       36 b- defN 24-Apr-06 12:47 kolibri/task/text/spelling/brillmoore/__init__.py
+-rw-r--r--  2.0 unx    10769 b- defN 24-Apr-06 12:47 kolibri/task/text/spelling/brillmoore/error_model.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 12:47 kolibri/task/text/spelling/electors/__init__.py
+-rw-r--r--  2.0 unx     2815 b- defN 24-Apr-06 12:47 kolibri/task/text/spelling/electors/kenlm_elector.py
+-rw-r--r--  2.0 unx     1421 b- defN 24-Apr-06 12:47 kolibri/task/text/spelling/electors/top1_elector.py
+-rw-r--r--  2.0 unx       61 b- defN 24-Apr-06 12:47 kolibri/task/text/spelling/levenshtein/__init__.py
+-rw-r--r--  2.0 unx    33386 b- defN 24-Apr-06 12:47 kolibri/task/text/spelling/levenshtein/levenshtein_searcher.py
+-rw-r--r--  2.0 unx     3406 b- defN 24-Apr-06 12:47 kolibri/task/text/spelling/levenshtein/searcher_component.py
+-rw-r--r--  2.0 unx    20586 b- defN 24-Apr-06 12:47 kolibri/task/text/spelling/levenshtein/tabled_trie.py
+-rw-r--r--  2.0 unx      152 b- defN 24-Apr-06 12:47 kolibri/task/text/topics/__init__.py
+-rw-r--r--  2.0 unx     3563 b- defN 24-Apr-06 12:47 kolibri/task/text/topics/baseTopic.py
+-rw-r--r--  2.0 unx    24958 b- defN 24-Apr-06 12:47 kolibri/task/text/topics/mallet.py
+-rw-r--r--  2.0 unx    14855 b- defN 24-Apr-06 12:47 kolibri/task/text/topics/topics_estimator.py
+-rw-r--r--  2.0 unx       58 b- defN 24-Apr-06 12:47 kolibri/task/timeseries/__init__.py
+-rw-r--r--  2.0 unx    23782 b- defN 24-Apr-06 12:47 kolibri/task/timeseries/dataset.py
+-rw-r--r--  2.0 unx      962 b- defN 24-Apr-06 12:47 kolibri/task/timeseries/metrics.py
+-rw-r--r--  2.0 unx     1953 b- defN 24-Apr-06 12:47 kolibri/task/timeseries/analysis/__init__.py
+-rw-r--r--  2.0 unx     7234 b- defN 24-Apr-06 12:47 kolibri/task/timeseries/analysis/eda_utils.py
+-rw-r--r--  2.0 unx    17003 b- defN 24-Apr-06 12:47 kolibri/task/timeseries/analysis/plotters.py
+-rw-r--r--  2.0 unx      494 b- defN 24-Apr-06 12:47 kolibri/task/timeseries/analysis/feature_relevance/__init__.py
+-rw-r--r--  2.0 unx     3066 b- defN 24-Apr-06 12:47 kolibri/task/timeseries/analysis/feature_relevance/relevance.py
+-rw-r--r--  2.0 unx     2919 b- defN 24-Apr-06 12:47 kolibri/task/timeseries/analysis/feature_relevance/relevance_table.py
+-rw-r--r--  2.0 unx      583 b- defN 24-Apr-06 12:47 kolibri/task/timeseries/analysis/outliers/__init__.py
+-rw-r--r--  2.0 unx     5017 b- defN 24-Apr-06 12:47 kolibri/task/timeseries/analysis/outliers/density_outliers.py
+-rw-r--r--  2.0 unx    13178 b- defN 24-Apr-06 12:47 kolibri/task/timeseries/analysis/outliers/hist_outliers.py
+-rw-r--r--  2.0 unx     1878 b- defN 24-Apr-06 12:47 kolibri/task/timeseries/analysis/outliers/median_outliers.py
+-rw-r--r--  2.0 unx     2998 b- defN 24-Apr-06 12:47 kolibri/task/timeseries/analysis/outliers/prediction_interval_outliers.py
+-rw-r--r--  2.0 unx     3501 b- defN 24-Apr-06 12:47 kolibri/task/timeseries/analysis/outliers/sequence_outliers.py
+-rw-r--r--  2.0 unx     1585 b- defN 24-Apr-06 16:16 kolibri/tokenizers/__init__.py
+-rw-r--r--  2.0 unx     4690 b- defN 24-Mar-30 22:58 kolibri/tokenizers/bert_tokenizer.py
+-rw-r--r--  2.0 unx     3999 b- defN 24-Mar-30 22:58 kolibri/tokenizers/char_tokenizer.py
+-rw-r--r--  2.0 unx     7103 b- defN 24-Mar-30 22:58 kolibri/tokenizers/kolibri_tokenizer.py
+-rw-r--r--  2.0 unx     2361 b- defN 24-Mar-30 22:58 kolibri/tokenizers/multi_word_tokenizer.py
+-rw-r--r--  2.0 unx     2661 b- defN 24-Mar-30 22:58 kolibri/tokenizers/regex_tokenizer.py
+-rw-r--r--  2.0 unx      964 b- defN 24-Apr-02 16:05 kolibri/tokenizers/segtok_tokenizer.py
+-rw-r--r--  2.0 unx     1025 b- defN 24-Mar-30 22:58 kolibri/tokenizers/sentence_tokenizer.py
+-rw-r--r--  2.0 unx     2789 b- defN 24-Apr-02 15:40 kolibri/tokenizers/tokenizer.py
+-rw-r--r--  2.0 unx     6936 b- defN 24-Mar-30 22:58 kolibri/tokenizers/ugc_tokenizer.py
+-rw-r--r--  2.0 unx     2404 b- defN 24-Mar-30 22:58 kolibri/tokenizers/word_tokenizer.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 12:47 kolibri/tools/__init__.py
+-rw-r--r--  2.0 unx      411 b- defN 24-Apr-06 12:47 kolibri/tools/_regex.py
+-rw-r--r--  2.0 unx      841 b- defN 24-Apr-06 12:47 kolibri/tools/arxiv.py
+-rw-r--r--  2.0 unx     1208 b- defN 24-Apr-06 12:47 kolibri/tools/bing_search.py
+-rw-r--r--  2.0 unx     1441 b- defN 24-Apr-06 12:47 kolibri/tools/ddg_search.py
+-rw-r--r--  2.0 unx     2063 b- defN 24-Apr-06 12:47 kolibri/tools/gebbrisg_detector.py
+-rw-r--r--  2.0 unx     1231 b- defN 24-Apr-06 12:47 kolibri/tools/google_search.py
+-rw-r--r--  2.0 unx    25525 b- defN 24-Apr-06 12:47 kolibri/tools/keywords.py
+-rw-r--r--  2.0 unx      777 b- defN 24-Apr-06 12:47 kolibri/tools/openweathermap.py
+-rw-r--r--  2.0 unx      853 b- defN 24-Apr-06 12:47 kolibri/tools/pubmed.py
+-rw-r--r--  2.0 unx     1828 b- defN 24-Apr-06 12:47 kolibri/tools/regexes.py
+-rw-r--r--  2.0 unx    17263 b- defN 24-Apr-06 12:47 kolibri/tools/scanner.py
+-rw-r--r--  2.0 unx      690 b- defN 24-Apr-06 12:47 kolibri/tools/wikipedia.py
+-rw-r--r--  2.0 unx      699 b- defN 24-Apr-06 12:47 kolibri/tools/wolfram_alpha.py
+-rw-r--r--  2.0 unx    13056 b- defN 24-Apr-06 12:47 kolibri/tools/word_frequencies.py
+-rw-r--r--  2.0 unx     1447 b- defN 24-Apr-06 12:47 kolibri/tools/youtube_search.py
+-rw-r--r--  2.0 unx     5493 b- defN 24-Apr-06 12:47 kolibri/utils/__init__.py
+-rw-r--r--  2.0 unx    11199 b- defN 24-Apr-06 12:47 kolibri/utils/cm.py
+-rw-r--r--  2.0 unx     6904 b- defN 24-Apr-06 12:47 kolibri/utils/common.py
+-rw-r--r--  2.0 unx     3173 b- defN 24-Apr-06 12:47 kolibri/utils/config.py
+-rw-r--r--  2.0 unx    12009 b- defN 24-Apr-06 12:47 kolibri/utils/cross_validation.py
+-rw-r--r--  2.0 unx    14474 b- defN 24-Apr-06 12:47 kolibri/utils/distribution.py
+-rw-r--r--  2.0 unx      873 b- defN 24-Apr-06 12:47 kolibri/utils/environement.py
+-rw-r--r--  2.0 unx    12576 b- defN 24-Apr-02 16:27 kolibri/utils/file_utils.py
+-rw-r--r--  2.0 unx     3259 b- defN 24-Apr-06 12:47 kolibri/utils/language_info.py
+-rw-r--r--  2.0 unx      544 b- defN 24-Apr-06 12:47 kolibri/utils/log_normalizer.py
+-rw-r--r--  2.0 unx     5686 b- defN 24-Apr-06 12:47 kolibri/utils/mathext.py
+-rw-r--r--  2.0 unx     2904 b- defN 24-Apr-06 12:47 kolibri/utils/matrix.py
+-rw-r--r--  2.0 unx     3158 b- defN 24-Apr-06 12:47 kolibri/utils/nb_clusters.py
+-rw-r--r--  2.0 unx      631 b- defN 24-Apr-06 12:47 kolibri/utils/parallel.py
+-rw-r--r--  2.0 unx     2361 b- defN 24-Apr-06 12:47 kolibri/utils/progress_bar.py
+-rw-r--r--  2.0 unx     4577 b- defN 24-Apr-06 12:47 kolibri/utils/serializable.py
+-rw-r--r--  2.0 unx     2280 b- defN 24-Apr-06 12:47 kolibri/utils/spinner.py
+-rw-r--r--  2.0 unx     1252 b- defN 24-Apr-06 12:47 kolibri/utils/text_encoding.py
+-rw-r--r--  2.0 unx    28893 b- defN 24-Apr-06 12:47 kolibri/utils/timeseries_functions.py
+-rw-r--r--  2.0 unx    28840 b- defN 24-Apr-06 12:47 kolibri/utils/timeseries_functions_back.py
+-rw-r--r--  2.0 unx      547 b- defN 24-Apr-06 12:47 kolibri/utils/wrappers/__init__.py
+-rw-r--r--  2.0 unx     5589 b- defN 24-Apr-06 12:47 kolibri/utils/wrappers/arxiv.py
+-rw-r--r--  2.0 unx     3344 b- defN 24-Apr-06 12:47 kolibri/utils/wrappers/bing_search.py
+-rw-r--r--  2.0 unx     3330 b- defN 24-Apr-06 12:47 kolibri/utils/wrappers/duckduckgo_search.py
+-rw-r--r--  2.0 unx     4910 b- defN 24-Apr-06 12:47 kolibri/utils/wrappers/google_search.py
+-rw-r--r--  2.0 unx     2431 b- defN 24-Apr-06 12:47 kolibri/utils/wrappers/openweathermap.py
+-rw-r--r--  2.0 unx     5742 b- defN 24-Apr-06 12:47 kolibri/utils/wrappers/pupmed.py
+-rw-r--r--  2.0 unx     4035 b- defN 24-Apr-06 12:47 kolibri/utils/wrappers/wikipedia.py
+-rw-r--r--  2.0 unx     2000 b- defN 24-Apr-06 12:47 kolibri/utils/wrappers/wolfram_alpha.py
+-rw-r--r--  2.0 unx      347 b- defN 24-Apr-06 12:47 kolibri/vectordb/__init__.py
+-rw-r--r--  2.0 unx    16307 b- defN 24-Apr-06 12:47 kolibri/vectordb/base.py
+-rw-r--r--  2.0 unx    23410 b- defN 24-Apr-06 12:47 kolibri/vectordb/faiss.py
+-rw-r--r--  2.0 unx    21812 b- defN 24-Apr-06 12:47 kolibri/vectordb/redis.py
+-rw-r--r--  2.0 unx    12276 b- defN 24-Apr-06 12:47 kolibri/vectordb/sklearn.py
+-rw-r--r--  2.0 unx     1462 b- defN 24-Apr-06 12:47 kolibri/vectordb/utils.py
+-rw-r--r--  2.0 unx      204 b- defN 24-Apr-06 12:47 kolibri/vectordb/docarray/__init__.py
+-rw-r--r--  2.0 unx     6872 b- defN 24-Apr-06 12:47 kolibri/vectordb/docarray/base.py
+-rw-r--r--  2.0 unx     4062 b- defN 24-Apr-06 12:47 kolibri/vectordb/docarray/hnsw.py
+-rw-r--r--  2.0 unx     2416 b- defN 24-Apr-06 12:47 kolibri/vectordb/docarray/in_memory.py
+-rw-r--r--  2.0 unx      280 b- defN 24-Apr-06 12:47 kolibri/vectordb/docstore/__init__.py
+-rw-r--r--  2.0 unx      924 b- defN 24-Apr-06 12:47 kolibri/vectordb/docstore/arbitrary_fn.py
+-rw-r--r--  2.0 unx      694 b- defN 24-Apr-06 12:47 kolibri/vectordb/docstore/base.py
+-rw-r--r--  2.0 unx      973 b- defN 24-Apr-06 12:47 kolibri/vectordb/docstore/in_memory.py
+-rw-r--r--  2.0 unx     1376 b- defN 24-Apr-06 12:47 kolibri/vectordb/docstore/wikipedia.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-06 12:47 kolibri/visualizations/__init__.py
+-rw-r--r--  2.0 unx    53376 b- defN 24-Apr-06 13:31 kolibri/visualizations/classification_plots.py
+-rw-r--r--  2.0 unx    15746 b- defN 24-Apr-06 12:47 kolibri/visualizations/pipeline.py
+-rw-r--r--  2.0 unx    34807 b- defN 24-Apr-06 12:47 kolibri/visualizations/regression_plots.py
+-rw-r--r--  2.0 unx    15565 b- defN 24-Apr-06 12:47 kolibri/visualizations/utils.py
 -rw-r--r--  2.0 unx       52 b- defN 23-Jul-09 11:29 tests/__init__.py
--rw-r--r--  2.0 unx    20075 b- defN 23-Jul-09 11:29 tests/test_data_transformer.py
+-rw-r--r--  2.0 unx    20075 b- defN 23-Aug-26 16:58 tests/test_data_transformer.py
 -rw-r--r--  2.0 unx      960 b- defN 23-Jul-09 11:29 tests/test_pipeline.py
 -rw-r--r--  2.0 unx      557 b- defN 23-Jul-09 11:29 tests/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 tests/entities/__init__.py
 -rw-r--r--  2.0 unx     7812 b- defN 23-Jul-09 11:29 tests/entities/test.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 tests/optuna/__init__.py
 -rw-r--r--  2.0 unx        1 b- defN 23-Jul-09 11:29 tests/optuna/test_optuna.py
--rw-r--r--  2.0 unx        1 b- defN 23-Jul-09 11:29 tests/synthesizer/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 tests/synthesizer/data_modules/__init__.py
--rw-r--r--  2.0 unx     2865 b- defN 23-Jul-09 11:29 tests/synthesizer/data_modules/test_conditional.py
--rw-r--r--  2.0 unx     1131 b- defN 23-Jul-09 11:29 tests/synthesizer/data_modules/test_sampler.py
--rw-r--r--  2.0 unx     2949 b- defN 23-Jul-09 11:29 tests/synthesizer/data_modules/test_transformer.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 tests/synthesizer/layers/__init__.py
--rw-r--r--  2.0 unx     7960 b- defN 23-Jul-09 11:29 tests/synthesizer/layers/test_gen_activation.py
--rw-r--r--  2.0 unx     1429 b- defN 23-Jul-09 11:29 tests/synthesizer/layers/test_layer_utils.py
--rw-r--r--  2.0 unx     4793 b- defN 23-Jul-09 11:29 tests/synthesizer/layers/test_residual.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 tests/synthesizer/losses/__init__.py
--rw-r--r--  2.0 unx     1128 b- defN 23-Jul-09 11:29 tests/synthesizer/losses/test_conditional_loss.py
--rw-r--r--  2.0 unx      812 b- defN 23-Jul-09 11:29 tests/synthesizer/losses/test_gradient_penalty.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 tests/synthesizer/models/__init__.py
--rw-r--r--  2.0 unx     1214 b- defN 23-Jul-09 11:29 tests/synthesizer/models/test_critic.py
--rw-r--r--  2.0 unx     4972 b- defN 23-Jul-09 11:29 tests/synthesizer/models/test_generator.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 tests/synthesizer/synthesizer/__init__.py
--rw-r--r--  2.0 unx     4090 b- defN 23-Jul-09 11:29 tests/synthesizer/synthesizer/test_synthesizer.py
--rw-r--r--  2.0 unx    34572 b- defN 23-Aug-25 15:12 kolibri_light-0.2.5.dist-info/LICENCE.txt
--rw-r--r--  2.0 unx     5148 b- defN 23-Aug-25 15:12 kolibri_light-0.2.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-25 15:12 kolibri_light-0.2.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Aug-25 15:12 kolibri_light-0.2.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    68439 b- defN 23-Aug-25 15:12 kolibri_light-0.2.5.dist-info/RECORD
-705 files, 4531935 bytes uncompressed, 1194956 bytes compressed:  73.6%
+-rw-r--r--  2.0 unx        1 b- defN 23-Aug-26 16:58 tests/synthesizer/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-26 16:58 tests/synthesizer/data_modules/__init__.py
+-rw-r--r--  2.0 unx     2865 b- defN 23-Aug-26 16:58 tests/synthesizer/data_modules/test_conditional.py
+-rw-r--r--  2.0 unx     1131 b- defN 23-Aug-26 16:58 tests/synthesizer/data_modules/test_sampler.py
+-rw-r--r--  2.0 unx     2949 b- defN 23-Aug-26 16:58 tests/synthesizer/data_modules/test_transformer.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-26 16:58 tests/synthesizer/layers/__init__.py
+-rw-r--r--  2.0 unx     7960 b- defN 23-Aug-26 16:58 tests/synthesizer/layers/test_gen_activation.py
+-rw-r--r--  2.0 unx     1429 b- defN 23-Aug-26 16:58 tests/synthesizer/layers/test_layer_utils.py
+-rw-r--r--  2.0 unx     4793 b- defN 23-Aug-26 16:58 tests/synthesizer/layers/test_residual.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-26 16:58 tests/synthesizer/losses/__init__.py
+-rw-r--r--  2.0 unx     1128 b- defN 23-Aug-26 16:58 tests/synthesizer/losses/test_conditional_loss.py
+-rw-r--r--  2.0 unx      812 b- defN 23-Aug-26 16:58 tests/synthesizer/losses/test_gradient_penalty.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-26 16:58 tests/synthesizer/models/__init__.py
+-rw-r--r--  2.0 unx     1214 b- defN 23-Aug-26 16:58 tests/synthesizer/models/test_critic.py
+-rw-r--r--  2.0 unx     4972 b- defN 23-Aug-26 16:58 tests/synthesizer/models/test_generator.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-26 16:58 tests/synthesizer/synthesizer/__init__.py
+-rw-r--r--  2.0 unx     4090 b- defN 23-Aug-26 16:58 tests/synthesizer/synthesizer/test_synthesizer.py
+-rw-r--r--  2.0 unx    34572 b- defN 24-Apr-08 23:02 kolibri_light-0.3.0.dist-info/LICENCE.txt
+-rw-r--r--  2.0 unx     4840 b- defN 24-Apr-08 23:02 kolibri_light-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-08 23:02 kolibri_light-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 24-Apr-08 23:02 kolibri_light-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    76395 b- defN 24-Apr-08 23:02 kolibri_light-0.3.0.dist-info/RECORD
+780 files, 6218880 bytes uncompressed, 1561494 bytes compressed:  74.9%
```

## zipnote {}

```diff
@@ -108,14 +108,35 @@
 
 Filename: kolibri/backend/base/estimator.py
 Comment: 
 
 Filename: kolibri/backend/base/nn_model.py
 Comment: 
 
+Filename: kolibri/backend/bert4keras/__init__.py
+Comment: 
+
+Filename: kolibri/backend/bert4keras/backend.py
+Comment: 
+
+Filename: kolibri/backend/bert4keras/layers.py
+Comment: 
+
+Filename: kolibri/backend/bert4keras/models.py
+Comment: 
+
+Filename: kolibri/backend/bert4keras/ops.py
+Comment: 
+
+Filename: kolibri/backend/bert4keras/snippets.py
+Comment: 
+
+Filename: kolibri/backend/bert4keras/tokenizers.py
+Comment: 
+
 Filename: kolibri/backend/bn/BayesianModel.py
 Comment: 
 
 Filename: kolibri/backend/bn/BayesianNetwork.py
 Comment: 
 
 Filename: kolibri/backend/bn/CPD.py
@@ -303,14 +324,242 @@
 
 Filename: kolibri/backend/bn/structure/structure_model.py
 Comment: 
 
 Filename: kolibri/backend/generators/__init__.py
 Comment: 
 
+Filename: kolibri/backend/model_abstractions/__init__.py
+Comment: 
+
+Filename: kolibri/backend/model_abstractions/model_object.py
+Comment: 
+
+Filename: kolibri/backend/model_abstractions/model_params.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/__init__.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/class_utils.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/data.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/file_utils.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/inference_utils.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/optim.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/samplers.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/splitter.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/tokenization.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/training_utils.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/datasets/__init__.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/datasets/base.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/datasets/document_classification.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/datasets/sequence_labeling.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/embeddings/__init__.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/embeddings/base.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/embeddings/document.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/embeddings/image.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/embeddings/legacy.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/embeddings/token.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/embeddings/transformer.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/models/__init__.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/models/clustering.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/models/entity_linker_model.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/models/language_model.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/models/multitask_model.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/models/pairwise_classification_model.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/models/pairwise_regression_model.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/models/prefixed_tagger.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/models/regexp_tagger.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/models/sequence_tagger_model.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/models/tars_model.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/models/text_classification_model.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/models/text_regression_model.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/models/word_tagger_model.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/models/sequence_tagger_utils/__init__.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/models/sequence_tagger_utils/crf.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/models/sequence_tagger_utils/viterbi.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/nn/__init__.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/nn/decoder.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/nn/dropout.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/nn/model.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/nn/multitask.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/nn/recurrent.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/nn/distance/__init__.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/nn/distance/cosine.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/nn/distance/euclidean.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/nn/distance/hyperbolic.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/trainers/__init__.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/trainers/language_model_trainer.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/trainers/trainer.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/trainers/plugins/__init__.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/trainers/plugins/base.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/trainers/plugins/metric_records.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/trainers/plugins/functional/__init__.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/trainers/plugins/functional/anneal_on_plateau.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/trainers/plugins/functional/checkpoints.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/trainers/plugins/functional/linear_scheduler.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/trainers/plugins/functional/reduce_transformer_vocab.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/trainers/plugins/functional/weight_extractor.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/trainers/plugins/loggers/__init__.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/trainers/plugins/loggers/clearml_logger.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/trainers/plugins/loggers/log_file.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/trainers/plugins/loggers/loss_file.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/trainers/plugins/loggers/metric_history.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/trainers/plugins/loggers/tensorboard.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/trainers/plugins/loggers/wandb.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/visual/__init__.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/visual/activations.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/visual/manifold.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/visual/ner_html.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/visual/training_curves.py
+Comment: 
+
+Filename: kolibri/backend/pytorch/visual/tree_printer.py
+Comment: 
+
 Filename: kolibri/backend/sklearn/__init__.py
 Comment: 
 
 Filename: kolibri/backend/sklearn/extensions/__init__.py
 Comment: 
 
 Filename: kolibri/backend/sklearn/extensions/decision_tree_log_reg.py
@@ -615,71 +864,17 @@
 
 Filename: kolibri/backend/tensorflow/utils/data.py
 Comment: 
 
 Filename: kolibri/backend/tensorflow/utils/model.py
 Comment: 
 
-Filename: kolibri/backend/tensorflow/utils/multi_label.py
-Comment: 
-
 Filename: kolibri/backend/tensorflow/utils/serialize.py
 Comment: 
 
-Filename: kolibri/backend/torch/__init__.py
-Comment: 
-
-Filename: kolibri/backend/torch/base_model.py
-Comment: 
-
-Filename: kolibri/backend/torch/models.py
-Comment: 
-
-Filename: kolibri/backend/torch/utils.py
-Comment: 
-
-Filename: kolibri/backend/torch/golem_utils/__init__.py
-Comment: 
-
-Filename: kolibri/backend/torch/golem_utils/golem_model.py
-Comment: 
-
-Filename: kolibri/backend/torch/golem_utils/train.py
-Comment: 
-
-Filename: kolibri/backend/torch/golem_utils/utils.py
-Comment: 
-
-Filename: kolibri/backend/torch/layers/__init__.py
-Comment: 
-
-Filename: kolibri/backend/torch/layers/crf.py
-Comment: 
-
-Filename: kolibri/backend/torch/tasks/__init__.py
-Comment: 
-
-Filename: kolibri/backend/torch/tasks/text/__init__.py
-Comment: 
-
-Filename: kolibri/backend/torch/tasks/text/labeling/__init__.py
-Comment: 
-
-Filename: kolibri/backend/torch/tasks/text/labeling/bi_lstm_crf.py
-Comment: 
-
-Filename: kolibri/backend/torch/utils/__init__.py
-Comment: 
-
-Filename: kolibri/backend/torch/utils/lbfgsb_scipy.py
-Comment: 
-
-Filename: kolibri/backend/torch/utils/locally_connected.py
-Comment: 
-
 Filename: kolibri/bin/__init__.py
 Comment: 
 
 Filename: kolibri/bin/datasets_configs.json
 Comment: 
 
 Filename: kolibri/bin/kolibri-download.py
@@ -726,14 +921,17 @@
 
 Filename: kolibri/data/base_stream.py
 Comment: 
 
 Filename: kolibri/data/blob.py
 Comment: 
 
+Filename: kolibri/data/data_base.py
+Comment: 
+
 Filename: kolibri/data/dataset.py
 Comment: 
 
 Filename: kolibri/data/document.py
 Comment: 
 
 Filename: kolibri/data/downloader.py
@@ -759,14 +957,26 @@
 
 Filename: kolibri/data/text.py
 Comment: 
 
 Filename: kolibri/data/utils.py
 Comment: 
 
+Filename: kolibri/data/datasets/__init__.py
+Comment: 
+
+Filename: kolibri/data/datasets/base.py
+Comment: 
+
+Filename: kolibri/data/datasets/document_classification.py
+Comment: 
+
+Filename: kolibri/data/datasets/sequence_labeling.py
+Comment: 
+
 Filename: kolibri/data/format/__init__.py
 Comment: 
 
 Filename: kolibri/data/format/conll.py
 Comment: 
 
 Filename: kolibri/data/format/csv.py
@@ -1026,14 +1236,17 @@
 
 Filename: kolibri/features/text/tfidf_weighted_embedder.py
 Comment: 
 
 Filename: kolibri/features/text/embedders/__init__.py
 Comment: 
 
+Filename: kolibri/features/text/embedders/abstract_embedder.py
+Comment: 
+
 Filename: kolibri/features/text/embedders/base.py
 Comment: 
 
 Filename: kolibri/features/text/embedders/bow_embedder.py
 Comment: 
 
 Filename: kolibri/features/text/embedders/elmo_embedder.py
@@ -1050,14 +1263,17 @@
 
 Filename: kolibri/features/text/embedders/openai.py
 Comment: 
 
 Filename: kolibri/features/text/embedders/tensorflow_hub.py
 Comment: 
 
+Filename: kolibri/features/text/embedders/transformers_embedder.py
+Comment: 
+
 Filename: kolibri/features/timeseries/__init__.py
 Comment: 
 
 Filename: kolibri/features/timeseries/features_utils.py
 Comment: 
 
 Filename: kolibri/features/timeseries/ts_featurizer.py
@@ -1128,14 +1344,17 @@
 
 Filename: kolibri/indexers/label_indexer.py
 Comment: 
 
 Filename: kolibri/indexers/multi_content_indexer.py
 Comment: 
 
+Filename: kolibri/indexers/multi_label.py
+Comment: 
+
 Filename: kolibri/indexers/multi_target_indexer.py
 Comment: 
 
 Filename: kolibri/indexers/sequence_char_indexer.py
 Comment: 
 
 Filename: kolibri/indexers/sequence_indexer.py
@@ -1815,14 +2034,17 @@
 
 Filename: kolibri/tokenizers/multi_word_tokenizer.py
 Comment: 
 
 Filename: kolibri/tokenizers/regex_tokenizer.py
 Comment: 
 
+Filename: kolibri/tokenizers/segtok_tokenizer.py
+Comment: 
+
 Filename: kolibri/tokenizers/sentence_tokenizer.py
 Comment: 
 
 Filename: kolibri/tokenizers/tokenizer.py
 Comment: 
 
 Filename: kolibri/tokenizers/ugc_tokenizer.py
@@ -1896,14 +2118,17 @@
 
 Filename: kolibri/utils/distribution.py
 Comment: 
 
 Filename: kolibri/utils/environement.py
 Comment: 
 
+Filename: kolibri/utils/file_utils.py
+Comment: 
+
 Filename: kolibri/utils/language_info.py
 Comment: 
 
 Filename: kolibri/utils/log_normalizer.py
 Comment: 
 
 Filename: kolibri/utils/mathext.py
@@ -2094,23 +2319,23 @@
 
 Filename: tests/synthesizer/synthesizer/__init__.py
 Comment: 
 
 Filename: tests/synthesizer/synthesizer/test_synthesizer.py
 Comment: 
 
-Filename: kolibri_light-0.2.5.dist-info/LICENCE.txt
+Filename: kolibri_light-0.3.0.dist-info/LICENCE.txt
 Comment: 
 
-Filename: kolibri_light-0.2.5.dist-info/METADATA
+Filename: kolibri_light-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: kolibri_light-0.2.5.dist-info/WHEEL
+Filename: kolibri_light-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: kolibri_light-0.2.5.dist-info/top_level.txt
+Filename: kolibri_light-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: kolibri_light-0.2.5.dist-info/RECORD
+Filename: kolibri_light-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kolibri/VERSION

```diff
@@ -1 +1 @@
-0.2.5
+0.3.0
```

## kolibri/__init__.py

```diff
@@ -15,27 +15,31 @@
 
 
 
 
 import os
 import random
 from dotenv import load_dotenv
-
+from pathlib import Path
 if "pytest" in sys.argv or "pytest" in sys.modules or os.getenv("CI"):
     print("Setting random seed to 42")
     random.seed(42)
 
 # Load the users .env file into environment variables
 load_dotenv(verbose=True, override=True)
 
 del load_dotenv
 verbose=1
 
-from dotenv import load_dotenv
+cache_root = Path(os.getenv("KOLIBRI_CACHE_ROOT", Path(Path.home(), ".kolibri")))
 
+_arrow = " → "
+
+from dotenv import load_dotenv
+import kolibri.backend.pytorch
 # Load the users .env file into environment variables
 load_dotenv(verbose=True, override=True)
 
 del load_dotenv
 verbose=1
 
 # //////////////////////////////////////////////////////
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## kolibri/model_trainer.py

```diff
@@ -228,15 +228,15 @@
 
                     performance_data.columns=columns
                 elif predictions is not None and predictions.size >0 and (len(predictions.shape)==1 or predictions.shape[1]==1):
                     performance_data=pd.DataFrame(X)
                     performance_data['class']=y
                     performance_data['prediction']=predictions.reshape(-1, 1)[:,0]
                 if model_results is not None:
-                    avgs_dict_log = {k: v for k, v in model_results.loc["Mean"].items()}
+                    avgs_dict_log ={} #{k: v for k, v in model_results.loc["Mean"].items()}
                     log_plots=self.config["log-plots"]
                     data_frames=[performance_data]
                     if self.experiment_logger is not None:
                         print("Logging experiment...")
                         self.experiment_logger.log_model(
                             experiment=self,
                             model=self.pipeline,
@@ -248,15 +248,15 @@
                             model_fit_time=model_fit_time,
                             log_plots=log_plots,
                             experiment_custom_tags=None,
                             dataframes=data_frames,
                             tune_cv_results=None,
                             URI=None
                         )
-            if self.config["register-model"]:
+            if self.config["register-model"] and self.experiment_logger is not None:
                 model_name=self.config["model-name"]
                 if model_name is None:
                     model_name=self.pipeline.estimator.name
                 self.experiment_logger.register_model(model_name,artifact=self.config['artefacts-path'], registered_model_version_stage=self.config["model-stage"], archive_existing_versions=self.config["archive-exiting-versions"])
         self.train_time=time.time()-start_time,
 
         gc.collect()
```

## kolibri/autolearn/model_zoo/zoo_classifier.py

```diff
@@ -10,17 +10,20 @@
 from copy import deepcopy
 from kolibri.logger import get_logger
 from kolibri.config import TaskType
 from kdmt.objects import class_from_module_path
 from kolibri.evaluation.classifier_evaluator import ClassifierEvaluator
 import pandas as pd
 from tabulate import tabulate
+from kolibri.registry import register
 
 logger = get_logger(__name__)
 
+
+@register('ZooClassifier')
 class ZooClassifier(BaseClassifier):
 
     defaults =  {"fixed": {
             "default-params": None,
             "classifiers": "all",
             "fast-models-only": False,
             "task-type": TaskType.CLASSIFICATION
@@ -85,15 +88,15 @@
 
             if params["matrix"]!="sparse":
                 X = X.toarray()
             self.model=model
 
             model_results, runtime, model_fit_time, predictions=super().fit(X, y, X_validation, y_validation)
 
-            performace_score=model_results.loc['Mean'].to_dict()
+            performace_score=model_results
             performace_score["classif_name"] = params["name"]
             names.append(params["name"])
             self.performace_scores.append(performace_score)
             performace_score_pd=deepcopy(performace_score)
 
             pd_report_scores.append(performace_score_pd)
         scores = pd.DataFrame(pd_report_scores)
```

## kolibri/backend/base/base_classifier.py

```diff
@@ -156,15 +156,15 @@
         logger.info("Uploading results into container")
 
 
         if performace_scores is not None:
             # yellow the mean
             model_results_ = color_df(performace_scores, "yellow", indices, axis=1)
             model_results_ = model_results_.format(precision=self.get_parameter("round"))
-            self.display.display(model_results_)
+#            self.display.display(model_results_)
 
         # end runtime
         runtime_end = time.time()
         runtime = np.array(runtime_end - runtime_start).round(self.get_parameter("round"))
 
 
 
@@ -182,18 +182,18 @@
         predictions=np.array(predictions)
         if predictions.size>0 and len(predictions.shape)==1:
             self.y_pred=predictions
         else:
             self.y_pred= [] if predictions.size==0 else predictions[:,1:,].astype(np.float16)
         if self.get_parameter("evaluate-performance")==True:
             self.plotter = ClassificationPlots(y_true=self.y_true, y_pred=self.y_pred, labels_dict=self.indexer.idx2token, X=self.X, y=self.y_true, classifier=self.model)
-            self.performace_scores=performace_scores.loc[['Mean', 'Std']].to_dict()
+            performace_scores=performace_scores.loc[['Mean', 'Std']].to_dict()
     #        self.performace_scores['Confusion_matrix']=confusion_matrix(self.y_true,np.argmax(self.y_pred, axis=1))
-            self.performace_scores['Confusion_matrix']=ClassifierEvaluator.confusion_matrix(list(self.y_true), list(np.argmax(self.y_pred, axis=1)), list(self.indexer.idx2token.values())).to_dict()
-            self.performace_scores['Class_report']=classification_report(self.y_true, np.argmax(self.y_pred, axis=1), target_names=list(self.indexer.idx2token.values()))
+            performace_scores['Confusion_matrix']=ClassifierEvaluator.confusion_matrix(list(self.y_true), list(np.argmax(self.y_pred, axis=1)), list(self.indexer.idx2token.values())).to_dict()
+            performace_scores['Class_report']=classification_report(self.y_true, np.argmax(self.y_pred, axis=1), target_names=list(self.indexer.idx2token.values()))
 
         return performace_scores, runtime, model_fit_time, predictions
 
     def _get_models(self):
         from kolibri.backend.models import sklearn_classification_models
         return sklearn_classification_models
```

## kolibri/backend/base/base_estimator.py

```diff
@@ -286,22 +286,22 @@
         """
         avgs_dict = {}
         predictions = []
         model_fit_start = time.time()
         model_results = None
 
         if self.get_parameter("evaluate-performance"):
-            self.display.update_monitor(1, "Initializing CV")
+#            self.display.update_monitor(1, "Initializing CV")
 
             cv = self.fold_generator
 
-            self.display.update_monitor(
-                row_idx=1,
-                message=f"Fitting {cv} Folds"
-            )
+            # self.display.update_monitor(
+            #     row_idx=1,
+            #     message=f"Fitting {cv} Folds"
+            # )
             """
             MONITOR UPDATE ENDS
             """
 
             metrics = self._get_metrics()
             metrics_dict = dict([(k, v.scorer) for k, v in metrics.items()])
 
@@ -351,15 +351,15 @@
             avgs_dict = {}
             for k, v in metrics.items():
                 avgs_dict[v.display_name] = []
                 test_score = scores[f"test_{k}"] * (1 if v.greater_is_better else -1)
                 test_score = test_score.tolist()
                 avgs_dict[v.display_name] += [np.mean(test_score), np.std(test_score)]
 
-            self.display.move_progress()
+#            self.display.move_progress()
 
             logger.info("Creating metrics dataframe")
 
             if hasattr(cv, "n_splits"):
                 fold = cv.n_splits
             elif hasattr(cv, "get_n_splits"):
                 fold = cv.get_n_splits()
```

## kolibri/backend/bn/structure/nonlinear.py

```diff
@@ -26,16 +26,16 @@
 import logging
 import os
 import torch
 import torch.nn as nn
 import numpy as np
 
 from kolibri.backend.bn.structure.base import BaseLearner, Tensor
-from kolibri.backend.torch.models import MLPModel, SobolevModel, squared_loss
-from kolibri.backend.torch.utils.lbfgsb_scipy import LBFGSBScipy
+from kolibri.backend.pytorch.models import MLPModel, SobolevModel, squared_loss
+from kolibri.backend.pytorch.utils.lbfgsb_scipy import LBFGSBScipy
 
 
 
 np.set_printoptions(precision=3)
 
 
 class NotearsNonlinear(BaseLearner):
```

## kolibri/backend/tensorflow/utils/__init__.py

```diff
@@ -9,15 +9,14 @@
 import tensorflow as tf
 from typing import TYPE_CHECKING, Union
 from tensorflow.keras.utils import CustomObjectScope
 from ._load_demo import load_demo
 from kolibri.backend.tensorflow  import custom_objects
 from .data import get_list_subset
 from .data import unison_shuffled_copies
-from .multi_label import MultiLabelBinarizer
 from .serialize import load_data_object
 from .model import convert_to_saved_model
 
 if TYPE_CHECKING:
     from kolibri.backend.tensorflow.tasks.text.labeling import BaseLabelingModel
     from kolibri.backend.tensorflow.tasks.text.classification import BaseTextClassificationModel
```

## kolibri/data/utils.py

```diff
@@ -354,15 +354,15 @@
     :rtype: str
     """
     resource_name = normalize_resource_name(resource_name, True)
 
     # Resolve default paths at runtime in-case the user overrides
     # kolibri.data.path
     if paths is None:
-        paths = path
+        paths = path if isinstance(path, list) else [path]
 
     # Check if the resource name includes a zipfile name
     m = re.match(r"(.*\.(zip|t?gz))/?(.*)$|", resource_name)
     if m.groups() is not None:
         zipfile, zipentry,_ = m.groups()
 
     # Check each item in our path
```

## kolibri/indexers/label_indexer.py

```diff
@@ -18,22 +18,22 @@
         data = super(LabelIndexer, self).to_dict()
         data['config']['multi_label'] = self.multi_label
         return data
 
     def __init__(self,
                  multi_label: bool = False,
                  **kwargs: Any) -> None:
-        from kolibri.backend.tensorflow.utils import MultiLabelBinarizer
+        from kolibri.indexers.multi_label import MultiLabelBinarizer
         super(LabelIndexer, self).__init__(**kwargs)
         self.multi_label = multi_label
         self.multi_label_binarizer = MultiLabelBinarizer(self.token2idx)
 
     def build_vocab_generator(self,
                               generators) -> None:
-        from kolibri.backend.tensorflow.utils import MultiLabelBinarizer
+        from kolibri.indexers.multi_label import MultiLabelBinarizer
         if self.token2idx:
             return
 
         token2idx: Dict[str, int] = {}
         token2count: Dict[str, int] = {}
         for generator in generators:
             if self.multi_label:
```

## kolibri/task/text/classification/sklearn_estimator.py

```diff
@@ -1,11 +1,11 @@
 import copy
 
 import joblib
-from kolibri.backend.models import get_classification_model
+from kolibri.backend.models import get_model
 from kolibri.backend.base.estimator import BaseEstimator
 from kdmt.dict import update
 from kolibri.optimizers.optuna.objective import EstimatorObjective
 from kolibri.logger import get_logger
 logger = get_logger(__name__)
 
 class SklearnEstimator(BaseEstimator):
@@ -17,15 +17,15 @@
         "tunable": {
         }
     }
     def __init__(self, hyperparameters=None, classifier=None, indexer=None):
         """Construct a new class classifier using the sklearn framework."""
 
         super(SklearnEstimator, self).__init__(params=hyperparameters, classifier=classifier, indexer=indexer)
-        self.hyperparameters["tunable"]["model"] = get_classification_model(hyperparameters["model"])
+        self.hyperparameters["tunable"]["model"] = get_model(hyperparameters["model"])
         self.update_model_parameters()
         self.model=self.load_model_from_parameters(self.get_parameter("model"))[1]
         self.X_sampled=None
         self.y_sampled=None
 
         self._dask_client=None
```

## kolibri/tokenizers/__init__.py

```diff
@@ -1,14 +1,16 @@
 from kolibri.tokenizers.kolibri_tokenizer import KolibriTokenizer
 from kolibri.tokenizers.char_tokenizer import CharTokenizer
 from kolibri.tokenizers.regex_tokenizer import RegexpTokenizer
 from kolibri.tokenizers.word_tokenizer import WordTokenizer
 from kolibri.tokenizers.sentence_tokenizer import SentenceTokenizer
 from kolibri.tokenizers.ugc_tokenizer import UGCTokenizer
 from kolibri.tokenizers.bert_tokenizer import BertTokenizer
+from kolibri.tokenizers.segtok_tokenizer import SegtokTokenizer
+from kolibri.tokenizers.tokenizer import Tokenizer
 
 # Standard sentence tokenizer.
 def tokenize_sentences(text):
     """
     Return a sentence-tokenized copy of *text*,
     using NLTK's recommended sentence tokenizer
     (currently :class:`.PunktSentenceTokenizer`
```

## kolibri/tokenizers/tokenizer.py

```diff
@@ -71,7 +71,11 @@
             text=str(text).casefold()
         if self.get_parameter("normalize"):
             text = unicodedata.normalize('NFC', str(text))
         if self.get_parameter("remove-punctuation") :
             text = "".join([ch for ch in text if ch not in self.filters])
 
         return text
+
+    @property
+    def name(self) -> str:
+        return self.__class__.__name__
```

## kolibri/visualizations/classification_plots.py

```diff
@@ -1,11 +1,9 @@
 import matplotlib.pyplot as plt
-import pandas
 from numpy import newaxis, arange, argmin, unique, concatenate, zeros_like, argmax, linspace
-from scipy import interp
 from kolibri.utils.cm import plot_confusion_matrix_from_matrix
 from sklearn.preprocessing import label_binarize
 from sklearn.metrics import confusion_matrix, precision_recall_curve, auc, roc_curve, average_precision_score, classification_report
 import itertools
 from itertools import product, cycle
 import random
 from statistics import mean
@@ -350,15 +348,15 @@
 
         # Aggregate all false positive rates
         all_fpr = unique(concatenate([fpr[i] for i in range(self.n_classes)]))
 
         # Then interpolate all ROC curves at this points
         mean_tpr = zeros_like(all_fpr)
         for i in range(self.n_classes):
-            mean_tpr += interp(all_fpr, fpr[i], tpr[i])
+            mean_tpr += np.interp(all_fpr, fpr[i], tpr[i])
 
         # Average it and compute AUC
         mean_tpr /= self.n_classes
 
         fpr["macro"] = all_fpr
         tpr["macro"] = mean_tpr
         roc_auc["macro"] = auc(fpr["macro"], tpr["macro"])
@@ -1241,15 +1239,15 @@
 
         ax1.set_ylabel("Fraction of positives")
         ax1.set_ylim([0, 1])
         ax1.set_xlim([0, 1])
         ax1.legend(loc="lower right")
         ax1.set_title("Calibration plots (reliability curve)")
         ax1.set_facecolor("white")
-        ax1.grid(b=True, color="grey", linewidth=0.5, linestyle="-")
+        ax1.grid(True, color="grey", linewidth=0.5, linestyle="-")
         plt.tight_layout()
 
         return plt
```

## Comparing `kolibri/backend/tensorflow/utils/multi_label.py` & `kolibri/indexers/multi_label.py`

 * *Files identical despite different names*

## Comparing `kolibri_light-0.2.5.dist-info/LICENCE.txt` & `kolibri_light-0.3.0.dist-info/LICENCE.txt`

 * *Files identical despite different names*

## Comparing `kolibri_light-0.2.5.dist-info/RECORD` & `kolibri_light-0.3.0.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,52 @@
-kolibri/VERSION,sha256=HreJmlTkdJt_ywhyUjgSvJTj6zhNsDqi_aCQwJHDY90,5
-kolibri/__init__.py,sha256=rp2ruqTHPF1ixmEpkFigpRJEpNHQMtdQRimgupv6__A,4359
+kolibri/VERSION,sha256=VQYTU3_EiPOzcq90pAAYefASyEZbgW8bhcbTRGss-0k,5
+kolibri/__init__.py,sha256=Kj4Mdf5ZWI8E5q-2EZwaLyZxpQVOMwnXEH3BQY1nkYA,4514
 kolibri/app.py,sha256=b_vLL8hIcbXgW_F-zOQfllebEiN-VdHsN7nEivYkZBA,16782
 kolibri/config.py,sha256=L1xrnHExgtg3gjE-pl67-BsOTJCtd9a-Gk8cG9FOo6M,3190
 kolibri/config_loader.py,sha256=gsdbv6fd6DU0HHd8aSOOMnOJL5dZJy8_pP2fqBWH_os,1902
 kolibri/default_configs.py,sha256=dGMN3ps9j_GD5C2KVWN5kFhVsIRHY8j5m4LsM3d4Gto,3814
 kolibri/errors.py,sha256=w4CWaoHWprc4NwaG9OmG0QKy8TsjzW40wx6x_p24dT8,5968
 kolibri/logger.py,sha256=bfFKEoKSshW41L2TCOTRDM03uP0RKJJ6ksyjToYaoYc,795
 kolibri/metadata.py,sha256=N-y50guFW7JojwgP0A_sZh-PidHnDk6ih1a3f2qw3TI,2219
 kolibri/model_loader.py,sha256=8XgjKM-oJ0xqcg3qiZ8uxXIO8-oL3PiRAR47cpEnbiI,10923
-kolibri/model_trainer.py,sha256=4TNiqz2UEl8fNk-hsxHJ_vEeVE5STrT26pfVwHXJiPI,25966
+kolibri/model_trainer.py,sha256=HafhAML9-jlGHdSlLUqnBabzWcWK9tPQBNqCLqisG0o,26008
 kolibri/registry.py,sha256=24l7CETeYLPnUjqVFHfiB1sU6T0GAgs7RtZSwwglBPk,2763
 kolibri/requirements.txt,sha256=wl9k0zC_6wMrj1aajNJUdT6mLw9Ow7c-aiS4s_tDVzU,153
 kolibri/settings.py,sha256=3-sXHEqp36xsV7y0U5GNrc5vjaLGJY23IyYJc3xIgFw,2490
 kolibri/settings.yaml,sha256=SbFpPQw3EeZc0W7GF9oyzIPIbVXMBSn7OyFnTT-ndwM,457
 kolibri/types.py,sha256=owjp0xUWDyV6yN3zuAZ8zdouU6LUS47yH5N3vLhi8TQ,361
 kolibri/version.py,sha256=O9Da2-eXuC6viLld4Vv9fFKJbZiQtCyH3j5t_xQNx3g,166
 kolibri/api/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kolibri/api/classification/__init__.py,sha256=_a-0VMXP0GdHBVKAj29d7aip0jfl2j7_HU-C17YMHvQ,2707
 kolibri/autolearn/__init__.py,sha256=Rv8ku1zDQlJFmPGGJgFGuy2odOmhXqlCNLoLH_fOWxc,66
 kolibri/autolearn/metalearn/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kolibri/autolearn/metalearn/metafeature.py,sha256=wXK9VbJ0msW8V_Bwdq0Po4dNQ1GnH2Ix3jaTeBTjqKw,3125
 kolibri/autolearn/metalearn/metafeatures.py,sha256=d43ZAEYIvrdRLPu4tPNYh1A6PD9YAAUySLUommeyiwU,46866
 kolibri/autolearn/model_zoo/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-kolibri/autolearn/model_zoo/zoo_classifier.py,sha256=2RxezAcf3vbW3qwP4qKca_5ghh8HBVb813WFvAOTmPY,4737
+kolibri/autolearn/model_zoo/zoo_classifier.py,sha256=JN4FUM8xU5SCwd-4sxkK8JY-8UwU0C_lDDSi9noIpdY,4781
 kolibri/autolearn/model_zoo/zoo_estimator.py,sha256=4jgft1w073y0wVdHBDpCV391oznUyilBeBTfqmP8p0E,5834
 kolibri/autolearn/model_zoo/zoo_regressor.py,sha256=qw-NLhgR12JO7aKuqtisU7pItiJ1WFeUOMKiT80d62o,4246
 kolibri/automl/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kolibri/automl/data_inspection.py,sha256=vV2ShQbbCTzYfNuaTT86dxRHPxkgIREJuJ5szV3ecK0,15341
 kolibri/backend/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kolibri/backend/models.py,sha256=X_olXosRAjLWgMIjR5blSzvy-HK-UJTT2RlJr5PiYA0,6230
 kolibri/backend/base/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-kolibri/backend/base/base_classifier.py,sha256=LCn_OXNfrnHg4lqzCbg1vyXuS6PTdtajj_q5QvWsOl8,11844
+kolibri/backend/base/base_classifier.py,sha256=i-ZH5fw2HT5IctQ3VhRg2Bh297T_G_6rCu8WDSJDDP0,11830
 kolibri/backend/base/base_clustering.py,sha256=-qOmW2V1nZga_xmNYf66MSy20KjMRadc8JGpPujTHE0,3916
-kolibri/backend/base/base_estimator.py,sha256=8yzv6YLnZsprfxYxViMG2t13_BfwImIlq8p59qcwIA4,30797
+kolibri/backend/base/base_estimator.py,sha256=fF53FelhneXxrHS9WVVWalOy8B1CuEzJSIlDNrCaiZQ,30807
 kolibri/backend/base/base_regressor.py,sha256=-Fmmhr8xIjo5dAOG3REpn9qZ0Sc-KXC2YYg5RRzaa50,7418
 kolibri/backend/base/estimator.py,sha256=jqCjFFH3TvZspLJ1uzo2hDO_meLBNWCL4r59QCyNv0o,14321
 kolibri/backend/base/nn_model.py,sha256=Azfnt31dNnV7cpS1RvV3XGLNhRUGvqHSIkbaEKjKqYc,912
+kolibri/backend/bert4keras/__init__.py,sha256=ENBAPU5AzTeONvxOSMnvMytWA24K75bZVKDg2IM9W1c,148
+kolibri/backend/bert4keras/backend.py,sha256=uUseveWxNKyUijJjtHMW9KyWUvMJTOiG3PgRVcNfagw,20228
+kolibri/backend/bert4keras/layers.py,sha256=4u-1I0UNXsxyO2sK9YKEagnmUlLsFHh74DoDiXT_YqM,52339
+kolibri/backend/bert4keras/models.py,sha256=6aSxlQgI1N35w0W6UoRhdVcZjil2qRr-CM7oK_naOrA,123662
+kolibri/backend/bert4keras/ops.py,sha256=H1sbMv6WOJ5iGAB0rosPz9LoqdT0jS8knLRW_6XkFRU,30152
+kolibri/backend/bert4keras/snippets.py,sha256=hVSxhppzD8rpVSPxOYU_g2Bdmcgwrny28tDRMdwCqK4,27957
+kolibri/backend/bert4keras/tokenizers.py,sha256=9fhMKc9MuwJElrnfaNXVD8w3Wpf8XNFvH--T86xsD24,15504
 kolibri/backend/bn/BayesianModel.py,sha256=2MsqjQ-T-c2yucpATa5qQJFGvkmDD4o-nSII6GhhRhs,449
 kolibri/backend/bn/BayesianNetwork.py,sha256=o9io0ndF2_MAX-ka8SPMIkqtMgazwl4NOGBJc3Vprls,44071
 kolibri/backend/bn/CPD.py,sha256=NgnqTgX-Mff2DWs5-xHdiK00wNz6QPvJiZSrj3tzAd8,24029
 kolibri/backend/bn/ContinuousFactor.py,sha256=oYzPEf5Q2SwnPMakyrk92WJQindhP-YCKp-9BiNJOn0,8931
 kolibri/backend/bn/DAG.py,sha256=0Sm6db1YnPZjd5pqF882_nBzUFENlcvV02ap4CuEK34,40531
 kolibri/backend/bn/DiscreteFactor.py,sha256=U3dYFwSC_5l3gjLnVB41w93jtZrOcfk-3wMDb_tn-rE,28630
 kolibri/backend/bn/DynamicBayesianNetwork.py,sha256=AEOnPTAklDg_1TEN5dKbx3SFURED6u_qocTSgod3T0I,31370
@@ -92,19 +99,95 @@
 kolibri/backend/bn/structure/learn.py,sha256=CjM-CTEDmnYnT9faPPI3xsaY27VJyyKqdLtJxi52lhM,1989
 kolibri/backend/bn/structure/linear.py,sha256=hQZKQ0ZjbEs17z_5pdSKJ_v-_sdrjNYzyUpfcMIS0mI,7267
 kolibri/backend/bn/structure/low_rank.py,sha256=9sWiZCiiyrkP6Pq0kEVvCoYeJSFdIEWE34VlOlo0Sxg,7902
 kolibri/backend/bn/structure/no_tears.py,sha256=TywuREMPmoZMzNmo76VQ4nDX9dAoaIUWjFdc0TGFobs,22607
 kolibri/backend/bn/structure/no_tears_tf.py,sha256=_gSzC9gALIqnufrlgFloQdTVAoVBpno8rA5XIutVse4,2961
 kolibri/backend/bn/structure/no_tears_tf2.py,sha256=vHegAFKIhm-gzPanlSjdZNADSzESbengWQ9m5j8CGUE,1898
 kolibri/backend/bn/structure/no_tears_tf_bak.py,sha256=_gSzC9gALIqnufrlgFloQdTVAoVBpno8rA5XIutVse4,2961
-kolibri/backend/bn/structure/nonlinear.py,sha256=wsdBgGZEzzVYR63tbE2gq62zCWzh8u2-QRaNty6KyNY,8816
+kolibri/backend/bn/structure/nonlinear.py,sha256=KKGkgfmfFuv9dxXmNiScolZmmm_o_AW4wtvS_Tr9YbI,8820
 kolibri/backend/bn/structure/notears_tf2.py,sha256=arZKt0xa4rOHtheMaIe-1RgwtAH7WUR5N5LRsg7azWU,4376
 kolibri/backend/bn/structure/plot_dag.py,sha256=JyFCcgnR53yzAuxr8jJ3RHEw-KxKSA6C85Gp0n5ierc,4208
 kolibri/backend/bn/structure/structure_model.py,sha256=0IDc08xa5o-TygQ0iySFRPjXHFnpisMBRR0XUjsV1ls,13671
 kolibri/backend/generators/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+kolibri/backend/model_abstractions/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+kolibri/backend/model_abstractions/model_object.py,sha256=l69ka3VlcJlLZUb4sAUkYFTq2DmJ2v-EIY4Zk7mq7eo,7922
+kolibri/backend/model_abstractions/model_params.py,sha256=quoXN7aqV04BtHfrVW2FIRyGm5i-Y1h2XXlXg_JnxXg,3106
+kolibri/backend/pytorch/__init__.py,sha256=nk18vKnCr9E1Mu_FqK2pEe7IPfqxNkOhu1aeOLGKFYc,2611
+kolibri/backend/pytorch/class_utils.py,sha256=U_GrPjNhG-r6d8r2SMXYd77oSjUx5d9F5b5oRZWkPdU,618
+kolibri/backend/pytorch/data.py,sha256=krsTUgSP5kj6PGDaqYJSMzK7Wpj3vdoX44-jPPyA-1o,69867
+kolibri/backend/pytorch/file_utils.py,sha256=hui4dFiuUbV09TKniuU_Zun3o6PzzpEmu4b7OkcKEgg,13971
+kolibri/backend/pytorch/inference_utils.py,sha256=-HMgMu9n_5uNQXtPmOTNsQbdpDRZXdPfqfawvA2CJKU,12239
+kolibri/backend/pytorch/optim.py,sha256=LMiUa4dxH52iXxfd1uPJJIUahdgDNBcVxlUJogeiO30,10900
+kolibri/backend/pytorch/samplers.py,sha256=M1PRkwcnN_KPYD3azFzrt4wSGEplMxmtMMBlT5nHGbs,3674
+kolibri/backend/pytorch/splitter.py,sha256=_wPS9bF7bAJRMTlkOnY7xkSo6CE0Dkb2rdaerfQNZnk,8216
+kolibri/backend/pytorch/tokenization.py,sha256=GbMeCzqGICz52Lxl2L6i_nhSgYtuSOUnngRbJZuQhNM,9749
+kolibri/backend/pytorch/training_utils.py,sha256=TQWMy8taOyvT8X5ylWyPKEpQTJ_J45hEGwVVIMzcwJU,14087
+kolibri/backend/pytorch/datasets/__init__.py,sha256=UGCYhAvXRP8MKatUMwkMXPOrGF0snWTAN8NRMkm4iLU,4333
+kolibri/backend/pytorch/datasets/base.py,sha256=CYqEOAVWi7Z8ovg-8QC4oXRgfURZ1Yuv2HxTbGBOagk,9448
+kolibri/backend/pytorch/datasets/document_classification.py,sha256=Z01ZyrhUyJiGBpEAs-Ygxaf4v9ee1KRFbVzt8RAGUjk,91543
+kolibri/backend/pytorch/datasets/sequence_labeling.py,sha256=aICSryJgEi5XzhhK73h1rvBWpiD_Sz7VkHUQmpbHViY,202979
+kolibri/backend/pytorch/embeddings/__init__.py,sha256=66GF8LlPHhVyMQWhLXo8ExbbSw_J-Olq2fLIKi2fENI,2473
+kolibri/backend/pytorch/embeddings/base.py,sha256=1_JSaARJKrLoRsX23QX5z04eaSpwOaD1G4i05jgR6wE,8074
+kolibri/backend/pytorch/embeddings/document.py,sha256=2pRx4pFtuhIc4FPher-vULaFhHBSBRxAAW_mOEnPGkw,30840
+kolibri/backend/pytorch/embeddings/image.py,sha256=XKXIfqkY22N67tqsWNh0B_Br6dWSE0uU0RlLW24COj8,10954
+kolibri/backend/pytorch/embeddings/legacy.py,sha256=UNsXDLsLqgMsBSQa9Y-nD9wopdU1uu9KqS3CvcEv1YU,29250
+kolibri/backend/pytorch/embeddings/token.py,sha256=imdw2YRIQWLAg90A-CfuNEC9Mv67NdOnCLTOXWsYeiU,66585
+kolibri/backend/pytorch/embeddings/transformer.py,sha256=_B_8a5dYfiZAl4_vZTiPKW8mbvrTjY6_E4JLw-cqVDY,63311
+kolibri/backend/pytorch/models/__init__.py,sha256=4EfWAMe56AtE2hKVnS9KjM1cbUDE0XI7fdJvQGrFjPY,962
+kolibri/backend/pytorch/models/clustering.py,sha256=b-p73jargs9M5wiEerg3TIHM_B-OxKQrv743vV3aIgM,4416
+kolibri/backend/pytorch/models/entity_linker_model.py,sha256=FeNEpweBOBWN4Hc9pJTf4CmVsCcMy7gc2SOc9IsHcuA,10614
+kolibri/backend/pytorch/models/language_model.py,sha256=-dNlTL1gXnUUjdd3UD0Q6AOjVXDMUCr2zhEDEG3pDZ4,17176
+kolibri/backend/pytorch/models/multitask_model.py,sha256=DJHq1fplomlhQotMSTOuPGT_s2fBRxS7_o1_OOVhMiA,11042
+kolibri/backend/pytorch/models/pairwise_classification_model.py,sha256=589jIlpWR3m40AttM9fWTM82lsCZrjFnQkgwmEEzGg0,5672
+kolibri/backend/pytorch/models/pairwise_regression_model.py,sha256=oiTH51moH7oScJC6jhXPaqwfMYls1rBQcvUcYHCppWE,14086
+kolibri/backend/pytorch/models/prefixed_tagger.py,sha256=BA2ix8j64aJ20QHDUojpqVr1a3MOMEbfuoYQ3PR6RFg,13839
+kolibri/backend/pytorch/models/regexp_tagger.py,sha256=t-zBOtbKACVXUwPyl4CEYYqn8frW3c3bc2VZonilu1U,4987
+kolibri/backend/pytorch/models/sequence_tagger_model.py,sha256=Oa5kYNq3JAAYLXWfdBWdSMw6HLJfn-WIMOxRPry2FTA,44679
+kolibri/backend/pytorch/models/tars_model.py,sha256=OZWjCUgShFdikLJQYLTBjWwCTRknE2FXwngJv3YTzVg,41492
+kolibri/backend/pytorch/models/text_classification_model.py,sha256=-AYccnNW-ILWjWrGkFEXz-3xliOec7s_VI30YaaIJCA,5241
+kolibri/backend/pytorch/models/text_regression_model.py,sha256=Ei8cH1XBNGbmLrg8823qmvaVmRlv_wXoJ3vK4EV4FRA,9594
+kolibri/backend/pytorch/models/word_tagger_model.py,sha256=-Nqs8Ty1lKx5xnHl0KKbrjFrcM3F6EoM-LfKYCqAiJI,9898
+kolibri/backend/pytorch/models/sequence_tagger_utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+kolibri/backend/pytorch/models/sequence_tagger_utils/crf.py,sha256=PEORqJXeE_aCYjBjsfVqntjBZhe9mD9t-Gfu3iMz_-U,2216
+kolibri/backend/pytorch/models/sequence_tagger_utils/viterbi.py,sha256=CTGWRM0BCU3rCLVmunvsAdFLa087K3tdeX6PesSlbfc,11636
+kolibri/backend/pytorch/nn/__init__.py,sha256=D96QbrgCeG4_UTDIwRhG_gZ2dAf2ivvoMwNjY6C70TE,337
+kolibri/backend/pytorch/nn/decoder.py,sha256=pmisBGbQtjKtEI6vcafxzuB927nFc8XcWsRH98qKQaE,8788
+kolibri/backend/pytorch/nn/dropout.py,sha256=6HJG9E6PCxYk23F-0NpisZa6Fk8UaCVJQY-MweB4K9o,1747
+kolibri/backend/pytorch/nn/model.py,sha256=eKqmKte2RXM_HX2F6RXpna7w0R1eC8KVVEnML-5IPOk,42491
+kolibri/backend/pytorch/nn/multitask.py,sha256=B2bvzfofXwWTnRDwoil5sUP_FDoA8Mn9_srq6rS4es4,815
+kolibri/backend/pytorch/nn/recurrent.py,sha256=JnFOm003rQsQa_hYiWivMd2JX_lBMoNEk32wQv4ViD0,437
+kolibri/backend/pytorch/nn/distance/__init__.py,sha256=I6402vwzEcQJogMLnF43QWApYf4Gqy6S6dbF_pvvK_4,387
+kolibri/backend/pytorch/nn/distance/cosine.py,sha256=4O9xnkHhB-mT7YjAd3GX4j-NRcuzf3Kyec2s-lAk_XM,1191
+kolibri/backend/pytorch/nn/distance/euclidean.py,sha256=8WRMT2oK_881jPYCxde611xysIt0TBo096g5u6cxRQo,1838
+kolibri/backend/pytorch/nn/distance/hyperbolic.py,sha256=rhOcNwYeFbz1uHjxVK0wyII6ozp2tFHRXImgzIp3HBU,3718
+kolibri/backend/pytorch/trainers/__init__.py,sha256=M6sO42oCF2_NWSHDxdvsBCWSp0Eab29G4Bv2kYDmevA,169
+kolibri/backend/pytorch/trainers/language_model_trainer.py,sha256=vChlkumM2JeHpftDQaaG-6qmchjLE6Mexx4kceJNoAg,17302
+kolibri/backend/pytorch/trainers/trainer.py,sha256=DwymYiNbOkh1cnQGnDLEEcZ5_r_ESZspYekvOm_x5ow,39933
+kolibri/backend/pytorch/trainers/plugins/__init__.py,sha256=2NQzrZssYUq_ORl-5ypKCvYPIRjlRFS7dV1ab70HTB8,1092
+kolibri/backend/pytorch/trainers/plugins/base.py,sha256=tNEdF2k8K8-Zzmgncuj5SyE1VbzUzOsL-7pOPpyDP1o,8498
+kolibri/backend/pytorch/trainers/plugins/metric_records.py,sha256=sPvYyte8JhZB0fNtFFm8mBPJW37dP2ZpS0PQLuCSQoc,4386
+kolibri/backend/pytorch/trainers/plugins/functional/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+kolibri/backend/pytorch/trainers/plugins/functional/anneal_on_plateau.py,sha256=zJTSlWh3DY82PQvv_IqQGWYRsfZhshs2tlzdhGu1A5E,4279
+kolibri/backend/pytorch/trainers/plugins/functional/checkpoints.py,sha256=px9eQtw71w7UcjrIRAke9bP0KMtK2hHSmx4xyWITD_w,1340
+kolibri/backend/pytorch/trainers/plugins/functional/linear_scheduler.py,sha256=M1pnnbenZBCeAQsfWW7xs3DVsH9TWrlB24HZ6k2-89s,2389
+kolibri/backend/pytorch/trainers/plugins/functional/reduce_transformer_vocab.py,sha256=TKo6rYFUMjvmVrVUDIQ2PvtQcpplRAcxCX67qQDLL5U,3149
+kolibri/backend/pytorch/trainers/plugins/functional/weight_extractor.py,sha256=1rvIKhcR5NR5lE7t9W6n6r4TC5nWSNmOlCdcp4oBv88,971
+kolibri/backend/pytorch/trainers/plugins/loggers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+kolibri/backend/pytorch/trainers/plugins/loggers/clearml_logger.py,sha256=9MPPMqSQVO-6JaqYAPevpaMPpGvnPofd6fg28r-lAW4,1661
+kolibri/backend/pytorch/trainers/plugins/loggers/log_file.py,sha256=E7HFgKe79w9a87sfNbpBrX7MC9cuaTUMyvjZkYOSOns,817
+kolibri/backend/pytorch/trainers/plugins/loggers/loss_file.py,sha256=l4eu2rtunaEPwyIzC783f4-J2ibdpEf2lrafjTso1lg,4500
+kolibri/backend/pytorch/trainers/plugins/loggers/metric_history.py,sha256=v9hi4q2s8pF3b9CRhlYVNOvl_D--mZ_qBd75oLLB2Yo,1282
+kolibri/backend/pytorch/trainers/plugins/loggers/tensorboard.py,sha256=XxAYFrYi_SUBI62P2qLTYRZP2yXGLUM-bEZJSTB8eV4,2548
+kolibri/backend/pytorch/trainers/plugins/loggers/wandb.py,sha256=MKrLCY6R5OlxLubc4zbUS6UUn0MQjPEGqWvkiQ43EjM,2542
+kolibri/backend/pytorch/visual/__init__.py,sha256=Mz6w1ArysWL-DFVT7e8IbbtJ5CKVgbDHlcHMrqijk4U,111
+kolibri/backend/pytorch/visual/activations.py,sha256=joQrfXiZdYFc1ogsVR_mLJY624NOU35l_G3PbhW_1r0,1910
+kolibri/backend/pytorch/visual/manifold.py,sha256=VbNsq_rdidUDYLrQ51bAwinldWSFtbzBWsgYlB2dGbQ,3350
+kolibri/backend/pytorch/visual/ner_html.py,sha256=GGO1YdBnm8oHPIKmCu_58uwOaFsbzgexmFPIckLmG0Q,3133
+kolibri/backend/pytorch/visual/training_curves.py,sha256=41r2jcHbd2sNE4YswLjOiRRcWE4NrHob1yx7yI4bpdU,7528
+kolibri/backend/pytorch/visual/tree_printer.py,sha256=8d58zl6WuJ3LTfQSsD2FnMHO_KWVoAwqWJScpAHABRU,909
 kolibri/backend/sklearn/__init__.py,sha256=7aIw8aWCxKcGFPNfJHiqNxdIkDlO3f_FNOr4TVyX9-g,157
 kolibri/backend/sklearn/extensions/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kolibri/backend/sklearn/extensions/decision_tree_log_reg.py,sha256=s-JImpaPsxEfe5ywRXpeGXDrstVY_irVlXiRARBuB9c,18744
 kolibri/backend/sklearn/extensions/distributed_nn.py,sha256=iWW_5haFKBzCKqbirwi9306c0cW18JF9w0wJu9rPNyI,1100
 kolibri/backend/sklearn/extensions/lazy_learner.py,sha256=fmG4FGZAdajTpX8kzZda1CmZ2qfLWzdILv91btJbI-A,15651
 kolibri/backend/sklearn/extensions/lookup_learner.py,sha256=UI5scygVPd5fdBWsAv8w1ScZp9Fr9JOR3vzBLLCqX9c,14741
 kolibri/backend/sklearn/meta/__init__.py,sha256=YvrffJMeN_MHWddQAwtasEzhYfOp372p-9s1YLG_kxI,65
@@ -197,37 +280,19 @@
 kolibri/backend/tensorflow/tasks/text/labeling/bi_gru_model.py,sha256=0ShDFcG055PKuv3Ts95FFVdY4E_18adSDsjDAd8b8GU,2249
 kolibri/backend/tensorflow/tasks/text/labeling/bi_lstm_crf_model.py,sha256=aeTeNw48JIpMtIk-kFncPT7Aq4SBWYfIg57Epw5fHq0,2991
 kolibri/backend/tensorflow/tasks/text/labeling/bi_lstm_model.py,sha256=qenOQPwgH7alvjQB1usXOzVxjDpLHoXfna2wUipzZU4,2295
 kolibri/backend/tensorflow/tasks/text/labeling/cnn_lstm_model.py,sha256=iukD4J4IUU237iFUlI6DQJi4sJTbq3-kLX_WJYyoDrs,1440
 kolibri/backend/tensorflow/tasks/text/seq2seq/__init__.py,sha256=oAlC4r3AbO9F-FMU9BBU7_y08ytDLdFX_HbvEWsbgT4,84
 kolibri/backend/tensorflow/tasks/text/seq2seq/generator.py,sha256=Rj4vvPHgoSfRO1cL8XNsRtS4ecLWy7RIR0l-RcWdkZA,2443
 kolibri/backend/tensorflow/tasks/text/seq2seq/model.py,sha256=nY0eIEiPnE9Qf4AAVtacrgKCG8cNoocEwLCgM_zqbYI,13913
-kolibri/backend/tensorflow/utils/__init__.py,sha256=DzVFqcCWM7ufMbd5Nz3yVsbJT4GPU1SW5KJjOovBxso,1203
+kolibri/backend/tensorflow/utils/__init__.py,sha256=kAHADT6RcDJzp2fQgFlasu34FlpQZSHrHEtUFi6luGc,1158
 kolibri/backend/tensorflow/utils/_load_demo.py,sha256=zP1gwDXGjoMbZLihKfY2RQmBGmkOdxEhRK6jtjxPfmQ,740
 kolibri/backend/tensorflow/utils/data.py,sha256=-QbFsfR7mrkqT14XKiaeSIMpeLvxdzqNmcRdK-xsb3c,919
 kolibri/backend/tensorflow/utils/model.py,sha256=1wCouP0vRXvReR__qaCmyl6yrrotlcM7iDiBBt5kHqI,1629
-kolibri/backend/tensorflow/utils/multi_label.py,sha256=Tbdks_UaClvw73eaSi0TBdVxjKzfofBAtT5X_PGE3dQ,1131
 kolibri/backend/tensorflow/utils/serialize.py,sha256=7BNzozD9ri4SxwOpA86CBx6zOSo4Z1TUug8QhES-IFs,862
-kolibri/backend/torch/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-kolibri/backend/torch/base_model.py,sha256=iemXUwH_6oS-VTQvyZ9MII_4KiTgXdBJmJFhRfL7H44,12666
-kolibri/backend/torch/models.py,sha256=H_iE2AgsZ0YyquBfpY6TzqqYh1XfJM866pY40d2P1EI,8161
-kolibri/backend/torch/utils.py,sha256=-AcqQwgxtSmsC9ZBGkhBUiXb2slTE7-p-2vqGmfmw_o,305
-kolibri/backend/torch/golem_utils/__init__.py,sha256=-fATNCo203nO81sb36u7l2wxPeAoyI6K_rW0UP3EZfU,671
-kolibri/backend/torch/golem_utils/golem_model.py,sha256=sEMXtKXG1GQGm1BP2_2-BmY0wdf4ceXBSS3IZIvzbew,4438
-kolibri/backend/torch/golem_utils/train.py,sha256=apdo4cXdD8Ohdv-v2zp9Q3MhuSU71kV5UAAzPSm9qK4,2545
-kolibri/backend/torch/golem_utils/utils.py,sha256=Yer0BK5mJU4B0A4pqnlhAsoA_LlZ8g-9kuw19VEYYuo,1636
-kolibri/backend/torch/layers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-kolibri/backend/torch/layers/crf.py,sha256=ToesvgWmCuozItH5lyrh7rHAPlkke_jhkWQTqL7kEAI,5973
-kolibri/backend/torch/tasks/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-kolibri/backend/torch/tasks/text/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-kolibri/backend/torch/tasks/text/labeling/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-kolibri/backend/torch/tasks/text/labeling/bi_lstm_crf.py,sha256=sG-TaWrFUzqD8gvU4zBj6PaLGZQgViPXI58fCEfrzOU,1836
-kolibri/backend/torch/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-kolibri/backend/torch/utils/lbfgsb_scipy.py,sha256=GYuoBToii0T_pLBM5WQ5-UBACsbwD6wsYp0sOH_bwUU,4009
-kolibri/backend/torch/utils/locally_connected.py,sha256=Dbpobd6wAUDT6jKjaTASeSkqzOHCNVXnQpRohECX_g0,2864
 kolibri/bin/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kolibri/bin/datasets_configs.json,sha256=Kxp26pPdkKw0PMYBP0TrtXGYw76GrCKV3wceLMnYGF8,471
 kolibri/bin/kolibri-download.py,sha256=rNBRMaJqGe7CYu7PQ914JPm31KJFdwy86nQijNmXPIE,2731
 kolibri/callbacks/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kolibri/callbacks/base.py,sha256=cM92pM1jzFE-g1AfsR_dpmUzVkQ5g4N344g3RO0jxPY,536
 kolibri/callbacks/callbacks_manager.py,sha256=hYCMKjQRVsxH_e7sm4X3-ysv5tAlFCuHpSHZVt4jlqo,3298
 kolibri/core/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -238,25 +303,30 @@
 kolibri/core/pipeline.py,sha256=hHFjzCAMmMBIN86g0EU76s6Kkt18ocMqiiKOJVzHoIw,17570
 kolibri/core/serializable.py,sha256=swVmR9xjz3jS-9oAwXTP1HXk0VSdkLJ02bDiOipgZ7Q,2289
 kolibri/core/vocabulary.py,sha256=0UxUN6DU-1yI3Q0ZsZ_zXW7xCCLF1aCs6F4Bbbx7-EI,5771
 kolibri/data/__init__.py,sha256=GdTNFBgeFswt8c0lh4jMERjdgtHsbv4CltjSunnY7Ik,117
 kolibri/data/auto_downloader.py,sha256=4Sj3RrDSVIjUduox15o45BJNWpOW_p6DvvoNsjrNSmM,4452
 kolibri/data/base_stream.py,sha256=PPW9u8j5MZRi1ImThILOk_j323aDZPuULRbNYki3-Aw,2246
 kolibri/data/blob.py,sha256=z1dBN9Xrkr2JFg3tRM9wFth3ZA5JG6EdyDalqZIB6gI,4978
+kolibri/data/data_base.py,sha256=KLToEfqclbQKIE0Y65sTx2OenpVHG0dAQKw2nQMe42Q,67193
 kolibri/data/dataset.py,sha256=OrpruQm7e6UacDY2WEVhg8on7_ySzzIS72WqDLYWsCY,29540
 kolibri/data/document.py,sha256=0thot_UdGo7SE_fkQB75NA_GmSu2Ews-h12V40ms86s,234
 kolibri/data/downloader.py,sha256=THQtLJtNtHvjC7s-PaPp8KTudsuMubdmuLZE3kfdhcg,39086
 kolibri/data/file_stream.py,sha256=W8x64Tp8xVX2t0h7DDCW67pQ7gK9BTEclpY9DSGk2b0,10372
 kolibri/data/iterator.py,sha256=-ymNquPlYE35emY66yGvEUccb91S0bP4emj4CscRfLY,534
 kolibri/data/resources.py,sha256=_YBXQXvpEeCHbKAG24FkJsjE4hFX-lVeodFq9tiAGSc,743
 kolibri/data/schemes.py,sha256=KzxsSXR0mtvtCKOfXwNMggWGacy6l0850OCbb1wwgZ8,10130
 kolibri/data/settings.py,sha256=uIsB2x_nUF7HgV4X59OeS8ZWMerQUx_zgbz_P3IzZDY,42659
 kolibri/data/streams.py,sha256=k1xJjvS8k898DvQ2ysGR9nijKiuHTzx-pj8U6Bx4dGM,5610
 kolibri/data/text.py,sha256=XHJKENpOng8Z-qI_AqJe_IXvJtTTHOk-MYJp15mPtJU,7910
-kolibri/data/utils.py,sha256=qxB9YItSUuoecqcU-FxFlND62CuEldVmOg0j26NEXik,43985
+kolibri/data/utils.py,sha256=TblBaLetW9KCJdrQ0QsXA6UAM-kyIV5_QhM14oUov58,44023
+kolibri/data/datasets/__init__.py,sha256=CNoe5yPK-ALH3XV1qksjaNv5uVRDaY6kl9zfkju9jUY,3883
+kolibri/data/datasets/base.py,sha256=ENQ0I_wLMAgw4vZ1tFWw8wirKV008CnAjS9nYERR1DU,9397
+kolibri/data/datasets/document_classification.py,sha256=Rlp_EA5HgikdNT0VzEVpJbPbQGlMOl8XHfOz3zdLLA8,91465
+kolibri/data/datasets/sequence_labeling.py,sha256=_1IiRJzU92-_E6mx8Z_k5I2KNdwC74icjDG3IC03ogs,200111
 kolibri/data/format/__init__.py,sha256=uDK8Bs_c3O4o9znYhK7_huuU5PVF-UnoWmHUOLG8z1w,94
 kolibri/data/format/conll.py,sha256=6WoRsOLmh5lJxNqnDu72U1HzBoYjOO3HVz8dHew4Hyo,539
 kolibri/data/format/csv.py,sha256=Eh1PAmR0KymT2O91b5tSdz6kazgkYUzDWLQ8L-j2FpY,385
 kolibri/data/loaders/__init__.py,sha256=RFY2ruffuLI3HyffcciNSayEE14Kh8fxbGTa116JK_c,149
 kolibri/data/loaders/arxiv.py,sha256=eRtDWuZoi6_zWAqI6kgD6vrgZpIoZssN_tDS22ayJmk,960
 kolibri/data/loaders/base.py,sha256=trP2pKAKJNwgy9R4CZkMqpVzqRVnZj1y4bczAg6IjP0,2516
 kolibri/data/loaders/csv_loader.py,sha256=ZLzya45-yPUU1fBEoX4CEDZG_7SjX-IIcEDpGpoVjYI,2238
@@ -338,22 +408,24 @@
 kolibri/features/text/feature_functions.py,sha256=8yHQPqUpIvTD9BMk022fzT2gt3a7GDo4UOPQUDO8umY,8352
 kolibri/features/text/hashing_tfidf_vectorizer.py,sha256=w9qipim7EjjyQp0eCLojmt2KzWK0Ili4HLBrLoOWuOM,10000
 kolibri/features/text/text_features.py,sha256=xbSwlero_jBAXotzq76QdD0GMHcbNaEWkSnV8L6ePv0,5801
 kolibri/features/text/tf_idf_featurizer.py,sha256=KJ-83jIkbQASZT_DIm64sph-nxTfdGMCUEsZRI6uqEA,6336
 kolibri/features/text/tf_idf_topics_vectorizer.py,sha256=qtam33XebaraRSbTT1n-zAVvSIVr0-5GjUoPCxXl9v0,5853
 kolibri/features/text/tfidf_weighted_embedder.py,sha256=rG5GRZset6-Aut823fQp2bwBOr8jYVxydIG4BQWInc0,8121
 kolibri/features/text/embedders/__init__.py,sha256=wo9ZBw8yOosILo8DstG3CwiRAUWFMYj7zNav-KTM6jY,346
+kolibri/features/text/embedders/abstract_embedder.py,sha256=XR-6CWTBGXBPDB_Fv8CI1QbyVvXC63nvnrtLDKvDbcY,3700
 kolibri/features/text/embedders/base.py,sha256=_QMlSNhdpScR60MRA1xcxj6bKhSi6f38-VZGGMeyDPU,3709
 kolibri/features/text/embedders/bow_embedder.py,sha256=tfFMxTVN_CLxZnFeUs82ftnp-mR7hgnnbWX5H102wiM,1347
 kolibri/features/text/embedders/elmo_embedder.py,sha256=nXFKG-Bv4uYNC9ke6uY31qvf3u4qnd4SAszKUC57NCc,9928
 kolibri/features/text/embedders/fasttext_embedder.py,sha256=S5dSvUWjfR-xiW4MUR6TJ9Gzevn2dKKmxrKd1svpJyE,1568
 kolibri/features/text/embedders/glove_embedder.py,sha256=bvJCLA2HAC05x1aJpGcxMC3wXcGTgK-GoZR8RzSgyE4,2027
 kolibri/features/text/embedders/llamacpp.py,sha256=tvYZ3kCJiIl9X8PVi6akfBYw_9f785sPUa-d8gMoGSA,4096
 kolibri/features/text/embedders/openai.py,sha256=1wl9fVxSIVOTcK0-Et46kLiOU2BdJIfHd9Djky7oPgs,17705
 kolibri/features/text/embedders/tensorflow_hub.py,sha256=QZIZ7IUH2n33EOV7H6bHXx0QHwJ2kc-Zgbr6skacl1s,2466
+kolibri/features/text/embedders/transformers_embedder.py,sha256=cVtxlIa-XgJGNUQjL4GPppbQquExaqajJRiy3hOt6CE,4920
 kolibri/features/timeseries/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kolibri/features/timeseries/features_utils.py,sha256=ErwwBJds2M8ELkH5qmkU_EF-gftjDELJTC-EfGNrHlQ,31971
 kolibri/features/timeseries/ts_featurizer.py,sha256=AXx4RYzRve1rBnKRYKV9S5-wFjXvc4fSTyi5db6kBgs,10656
 kolibri/features/timeseries/utils.py,sha256=bBVaXfSmvxk7CHtQYOOoYzd1vNQzS4ZrxVfvkw-DtQU,7659
 kolibri/features/timeseries/feature_extraction/__init__.py,sha256=YK6iWKahGZ3sk6wCYkKtZB9Hsp6t0NlX4aTGBDvqSlE,358
 kolibri/features/timeseries/feature_extraction/data.py,sha256=iCxVcnnmHlYfiKeDqfRM-wsTmK4rV4L0HW5gVC8uEpc,16661
 kolibri/features/timeseries/feature_extraction/extraction.py,sha256=OG4h6ZRbNTb8LPq8gEX15gGpbt4Wr2bEZSFCE_AQINo,13772
@@ -370,16 +442,17 @@
 kolibri/formers/text/classifier.py,sha256=hC-1Mg4brwzxwbi4-WST5U35QXKsgMsRRarK-d1nNzk,4315
 kolibri/formers/text/sentiment.py,sha256=bDtublKNNJTK0ZLHPQy-VfSELx3swUnFFegDwV4Gllk,230
 kolibri/formers/text/similarity.py,sha256=XYWHPev_HliftwoieOhu8P1ylGlMVHXekyRi6nTh9IU,4515
 kolibri/formers/text/topic_former.py,sha256=vMKyUWLKM-PZC5U_w62YoGPpz32Rx1-XX5KNMlTRkwc,40754
 kolibri/indexers/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
 kolibri/indexers/base_indexer.py,sha256=74JKu3F-tH6IQP3nnfgnJHD6svAbtjL5lXScXCd7KUE,2657
 kolibri/indexers/kolibri_label_encoder.py,sha256=r6m52A_WH_r6pQ_H91CNjH9IfTU__9uFc2ID3fucOOY,1239
-kolibri/indexers/label_indexer.py,sha256=xmIq4iCE-M6KGCo0PzwWMuvKCEAM8E10mJLZhNN9npU,3490
+kolibri/indexers/label_indexer.py,sha256=YAjb-25iLBz76ovZoKE42PaHFdnDcX04oHK-wBZrFlk,3482
 kolibri/indexers/multi_content_indexer.py,sha256=v6NoarZ01DqWcVz5NvP2Te67cRU6VJGuEW2ElxyUEPk,1248
+kolibri/indexers/multi_label.py,sha256=Tbdks_UaClvw73eaSi0TBdVxjKzfofBAtT5X_PGE3dQ,1131
 kolibri/indexers/multi_target_indexer.py,sha256=w8a87da5TklAoT9UpKYae9IEKHTXXgHBf84hUCpanp4,2394
 kolibri/indexers/sequence_char_indexer.py,sha256=Dybu74o1NSKuumnJ12HhxJCUueoYQ6SjXYZVW36gAXA,4944
 kolibri/indexers/sequence_indexer.py,sha256=BuZ2ZnB5rGGRVVyIwwxte8ECUxPEAEjrfp_1BnQO0tg,6012
 kolibri/indexers/text_indexer.py,sha256=Oa9FLoh9tX_f2bmztV57CCzN9ick-xbVzCgzXb-C9-s,5940
 kolibri/knowledge/__init__.py,sha256=xN5_d2ADMEkBYwdXEs6g_YXbRQZj5g6puJkqdIJoiWY,43
 kolibri/knowledge/domain.py,sha256=4QZoMJ1_8x1heIqs_lhNLbZHqRGob7HCteEJCRHiwwA,1173
 kolibri/llms/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -524,15 +597,15 @@
 kolibri/task/tabular/regression/sklearn_regression_estimator.py,sha256=JEEASNhXcoykxcLPDTLyrBY0JliIhmN2-wZ6upF5Jt4,2171
 kolibri/task/tabular/rulemining/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kolibri/task/tabular/rulemining/association_rules.py,sha256=_9mMxCmc8f6J6Cr_532xNVbtgVNVuTRJ_EMQTR8AgEY,9912
 kolibri/task/text/__init__.py,sha256=wy0HhZdrwePNnZIxZJFeQepcRweCbIuB7_v8ZS_e3ak,140
 kolibri/task/text/classification/__init__.py,sha256=YrTKGSQR4ykA_15LIkdMlRsOKwcQJJst0n056gXxUx4,190
 kolibri/task/text/classification/dnn_classification_estimator.py,sha256=B9vKwuxJQFR0N-HVDNsmczopwsq5JfmW2bq73XfSeOI,4316
 kolibri/task/text/classification/sklearn_classification_estimator.py,sha256=As4q2fhbjSNu6FB-MGWjgyr-OsQknpGmcOMYMCS2z0Q,3199
-kolibri/task/text/classification/sklearn_estimator.py,sha256=F_N3KjStwtKWwvt9i7hDqI2uzIOREpUI-Ii8bthIbm8,3292
+kolibri/task/text/classification/sklearn_estimator.py,sha256=Pw5djNBIH-7h1ZqP6IF2_e09upEDFdHembxjV6hKxVE,3262
 kolibri/task/text/entities/__init__.py,sha256=SKUlmOOjZ4Xl7bX8aQjhdprL-nAMmTxiSKc7FhRs3AY,3145
 kolibri/task/text/entities/common_reg_extractor.py,sha256=za0fjoLJuthsD6HIS8RiC5RXzZMOUPJx9TKPZJh6_zM,1990
 kolibri/task/text/entities/crf_entity_extractor.py,sha256=5IGuKTVmYifF2VISf2zc824qTOQVgdFESKGMo9wSE6M,17418
 kolibri/task/text/entities/dictionaryExtractor.py,sha256=3w-VRkpc-QH0skCRGr_chtKdOPSJC3ISeyt6ddcfEnw,949
 kolibri/task/text/entities/entity.py,sha256=yZxwmhwauYfjV-XNJ7Oot2VxlkoZACGcpHvetsQfb0E,1111
 kolibri/task/text/entities/entity_extractor.py,sha256=qSync2Cz2CM_uc9ldIU0KTGKiiVKeyJc8NgYETl43Kg,3007
 kolibri/task/text/entities/entity_synonyms.py,sha256=aSjkSDcggx35BVM9BFoqZOHJ8UP3DaioSZUfULoGGdk,4171
@@ -595,22 +668,23 @@
 kolibri/task/timeseries/analysis/feature_relevance/relevance_table.py,sha256=VvtAdg0v5QlqnKCtSIuZs5FQgX3P7IhdKsyxhozVmtE,2919
 kolibri/task/timeseries/analysis/outliers/__init__.py,sha256=KXxUdUXCOAey8kkK_CZpdYcsqjbt5HEMs_mI7Wb-bK0,583
 kolibri/task/timeseries/analysis/outliers/density_outliers.py,sha256=NLjzCKwrDvIUS5Y1hh7Bd74bu48Ok4BJ57E67c6mAU8,5017
 kolibri/task/timeseries/analysis/outliers/hist_outliers.py,sha256=lRVmbNYAvSjTmYKbiKXFFHZb4w2DDryrRU9_JiHKQsE,13178
 kolibri/task/timeseries/analysis/outliers/median_outliers.py,sha256=LOIVmtYKezbFcfM0gZqztPqEx56sWy7O0gDgyeeyg5A,1878
 kolibri/task/timeseries/analysis/outliers/prediction_interval_outliers.py,sha256=Kap9gxlRsKKyxoHqwsd74RBN9f1XO3YFr7cMlyF21XU,2998
 kolibri/task/timeseries/analysis/outliers/sequence_outliers.py,sha256=PiaW43p09ATc0P9dYIEKztiIqQoP2bw3q60YnHEJlPQ,3501
-kolibri/tokenizers/__init__.py,sha256=Jj-Y5GOcx1YNO-gf9yajTbW4hCNE15lWexB5JgHOxN0,1470
+kolibri/tokenizers/__init__.py,sha256=ERvx7kNNdueZk-FQCDddmkAN1erZ0H3JtEUno8U--O4,1585
 kolibri/tokenizers/bert_tokenizer.py,sha256=IqspexqV_7byM3UvdYRU8TIgoL6ycfAdZs0M6dcImQI,4690
 kolibri/tokenizers/char_tokenizer.py,sha256=YevabURuHJ716HKCWiiORZHc_Cs9KDeDx7_3c5MLoDI,3999
 kolibri/tokenizers/kolibri_tokenizer.py,sha256=ofvGQVkI6lC7nhIwViYHDceVptTFwhbKOJmwr2sZMts,7103
 kolibri/tokenizers/multi_word_tokenizer.py,sha256=jt9WQPm3OrK7m77CFVZ0seUlI_e5U0TkaJkNGoa5k1c,2361
 kolibri/tokenizers/regex_tokenizer.py,sha256=tHtenqZnad4gD1kPGj1A3Zm7nm8_XMiBIJzyx5RqXJA,2661
+kolibri/tokenizers/segtok_tokenizer.py,sha256=ZhTtc-LmUYwCkeILAFOXXwfBNlJaUt5EXGDSQCiJN20,964
 kolibri/tokenizers/sentence_tokenizer.py,sha256=1obx34ndBgLP3oipTAgCpiVtnUJgBRTYqYYB4gN4WzU,1025
-kolibri/tokenizers/tokenizer.py,sha256=So7J0D02ib0-tRZzuIXj4cggVsZyv3iGt8iyv1KDNXc,2708
+kolibri/tokenizers/tokenizer.py,sha256=ZT5L8wzddoKYo2WxY0gn_dvb-ZdBTcGpd2J80hwGa8E,2789
 kolibri/tokenizers/ugc_tokenizer.py,sha256=-Ja9ICY5mgwaLb09B6RvXRTlF2Ao5j17VZcvTBDIZUk,6936
 kolibri/tokenizers/word_tokenizer.py,sha256=D-aYGuTFpwK9vEZaSwW0sorhg7WgGHeJNMKZ-bGJig4,2404
 kolibri/tools/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kolibri/tools/_regex.py,sha256=4xOVvbQMT7mF4Lk8VbaBQ1jxovHd8irZMfT-4BdnDhM,411
 kolibri/tools/arxiv.py,sha256=B0xvh51ZX6_1_ix8_JdHwIwGEbXMra9yOI4VWdTT0rM,841
 kolibri/tools/bing_search.py,sha256=84MmQav3HKN1DifgVfWK4xgBLljueYGQKGQFGEr6570,1208
 kolibri/tools/ddg_search.py,sha256=um7jz6HUmyRDSfF7p7v8Jg58KvpcYaDVoMbEmwiIsGs,1441
@@ -628,14 +702,15 @@
 kolibri/utils/__init__.py,sha256=Rw6Z5th52gRopVPdS06kw48oeAQsHhQuu0_QoKEFe2g,5493
 kolibri/utils/cm.py,sha256=v3mEmruvlWXQLWSxZ19a8SPe_sKgnQQWb-Y4WUbFnM0,11199
 kolibri/utils/common.py,sha256=c3razuYtX7ELiRYNTSEXQXpBSq81ssWg9u3iZsKzzcY,6904
 kolibri/utils/config.py,sha256=qmcpjeS9B9J8zcKV79Wd4nmL_urBj_h-vTAIX8fowkM,3173
 kolibri/utils/cross_validation.py,sha256=oxYpuuEhHMEcVLx0g0EZ0AuppyZMBRO3-mtdpnZT3RA,12009
 kolibri/utils/distribution.py,sha256=rJFXEUUgixpyueTBH6ZHlbq0Uig1-LvHkEVg48sr76U,14474
 kolibri/utils/environement.py,sha256=IB9Cp5DrBy1RrPqHKix9mUVVWhUA0Aji8Imy3WydxX8,873
+kolibri/utils/file_utils.py,sha256=mBnO5f63_1klQBVmCGWdovnT_1t7ULM7xl5-jRQiqRQ,12576
 kolibri/utils/language_info.py,sha256=MxLTC_9odTRgNKDgN_w4mrMEYuWyfih_dxwGTwAUW64,3259
 kolibri/utils/log_normalizer.py,sha256=jiqdte_24Ge1I9qVme4nBa4X8jikzgydGqKBsbobEt4,544
 kolibri/utils/mathext.py,sha256=wBa1EobE3bzdQqPfTA71c8eNKtiirJd5rD5hhm0gP5U,5686
 kolibri/utils/matrix.py,sha256=8N-2XU398bUxonr7n2vlST9mXe4qEFYCVAGTEWH56Jg,2904
 kolibri/utils/nb_clusters.py,sha256=V485u3qTggAhVKUIHgFw7OqfXgl3Q7DdVk8APvB8VYw,3158
 kolibri/utils/parallel.py,sha256=da-WNpIKjaqqprIQmiWHDqjG1fa5ZXKv8K4SEDcqPDA,631
 kolibri/utils/progress_bar.py,sha256=Ket95lzKqFnGn5VffYqu1pDkUI6MlXduhZTI7-3i3sQ,2361
@@ -665,15 +740,15 @@
 kolibri/vectordb/docarray/in_memory.py,sha256=lkMYlJHssuAc4ZI7ia_UsfKLSdXbOyAFoyjbD0yONmw,2416
 kolibri/vectordb/docstore/__init__.py,sha256=uP5oA4wBVJ3P-tMqF_dAyZ0aSpLIFKNpXe7WtSGVgfQ,280
 kolibri/vectordb/docstore/arbitrary_fn.py,sha256=t36gwb_lJ8ng68Q4h5OIxCbuM8P-39A1eRuUSvbLkpA,924
 kolibri/vectordb/docstore/base.py,sha256=FKOH5Pgty0KxQu9fTNpK7CdH7khNvClOF5HJPq2leaY,694
 kolibri/vectordb/docstore/in_memory.py,sha256=PYDLIdJ4PJOEM9rpyd04nSxFghc75CzTBDspSaX5a4o,973
 kolibri/vectordb/docstore/wikipedia.py,sha256=E0cNtCh1Cvio_Qm54soJT8AiJZsO98NniATF63wtVtc,1376
 kolibri/visualizations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-kolibri/visualizations/classification_plots.py,sha256=uQMLdKu4jQ6dsomcGuG8PkGF1JkRhoBYyyz9ja_9-nM,53414
+kolibri/visualizations/classification_plots.py,sha256=BCIgYvKmHZojE9NnDZdQ6IKtIdVKgdKrCkdjoGxnXlk,53376
 kolibri/visualizations/pipeline.py,sha256=KXNnLW2yfzSosb_CcZX3KttAnFhqKi20ZZvqMqMFhZU,15746
 kolibri/visualizations/regression_plots.py,sha256=DcD7i6Q8CV9Qqc1g_uFvBfOOBZOROpI_k5MSnBakzzg,34807
 kolibri/visualizations/utils.py,sha256=YWNyh28EY6QcQ11cr2i72LiEv1cj9MBhJgv3-aEuXJw,15565
 tests/__init__.py,sha256=cLEG0Ty3GCvE16djVZjDu8rlBEUAVjwMZXa9fQlxVt0,52
 tests/test_data_transformer.py,sha256=Wy8Uqsl0DAzcOyn1-IYWEa1hHcMoy_eQUx9DBSwqJNc,20075
 tests/test_pipeline.py,sha256=BhvJX-IqJ_5EWnVj-VfXiM2LzR3-y9DGf3hZEaxEs50,960
 tests/utils.py,sha256=vvK537soXHoQnfBgTZw7yAtUjMO0pUWSSLcy8fH1pEg,557
@@ -694,12 +769,12 @@
 tests/synthesizer/losses/test_conditional_loss.py,sha256=0M-0-jADLCloslFs13GBqpLch_qvH7hatu3VvnaebhE,1128
 tests/synthesizer/losses/test_gradient_penalty.py,sha256=59gDBEWqfW91QiijmW1oAZJNY_r0T8lu2CINX-z_bhU,812
 tests/synthesizer/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/synthesizer/models/test_critic.py,sha256=A3Kgay2o4n0HkbIu9n1TDxRMw8G37r3HLdhb2qh0eSk,1214
 tests/synthesizer/models/test_generator.py,sha256=RI3E5_RKcCxnMSN4y0am6ar4ey-pxp5DQ8_LhHXa4ZQ,4972
 tests/synthesizer/synthesizer/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/synthesizer/synthesizer/test_synthesizer.py,sha256=qfsM8Okg8bW8V5NTKe657OiBFc7xKcD2dvkbqFm3_qg,4090
-kolibri_light-0.2.5.dist-info/LICENCE.txt,sha256=eKw0ToK5-JtbuPy1tofBiXFxGgk1zhq5x0mB7gnTxc8,34572
-kolibri_light-0.2.5.dist-info/METADATA,sha256=lKtiLX067C81ln7AhZPgBMJKiHx4AqytkunWSYovvbA,5148
-kolibri_light-0.2.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-kolibri_light-0.2.5.dist-info/top_level.txt,sha256=yZ09x7U41HE_HCr8pIum9-4eicynuHE26_L6DqI97b8,14
-kolibri_light-0.2.5.dist-info/RECORD,,
+kolibri_light-0.3.0.dist-info/LICENCE.txt,sha256=eKw0ToK5-JtbuPy1tofBiXFxGgk1zhq5x0mB7gnTxc8,34572
+kolibri_light-0.3.0.dist-info/METADATA,sha256=hklliuiowLHWEyfopOQf3aHR2iFvFUMFVw__bgKF23I,4840
+kolibri_light-0.3.0.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+kolibri_light-0.3.0.dist-info/top_level.txt,sha256=yZ09x7U41HE_HCr8pIum9-4eicynuHE26_L6DqI97b8,14
+kolibri_light-0.3.0.dist-info/RECORD,,
```

