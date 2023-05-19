##This is for the config for DoppelGANger. Use these values on the loaded data or it will not train.


    "global_config": {
        "batch_size": 3,
        "vis_freq": 200,
        "vis_num_sample": 5,
        "d_rounds": 1,
        "g_rounds": 1,
        "num_packing": 1,
        "noise": True,
        "feed_back": True,
        "g_lr": 0.001, #was 0.001
        "d_lr": 0.001,#was 0.001
        "d_gp_coe": 10.0, #was 10
        "gen_feature_num_layers": 1, #was 1
        "gen_feature_num_units": 100, #was 100
        "gen_attribute_num_layers": 3, #was 3
        "gen_attribute_num_units": 100, #was 100
        "disc_num_layers": 5, #was 5
        "disc_num_units": 200, #was 200
        "initial_state": "zero", #was random

        "attr_d_lr": 0.001,#was 0.001
        "attr_d_gp_coe": 10., #was 10
        "g_attr_d_coe": 1.0,
        "attr_disc_num_layers": 5, #was 5
        "attr_disc_num_units": 200, #was 200
    },

    "test_config": [
        {
            "dataset": ["#####DATANAME#######"],
            "epoch": [400],
            "run": ["0"],
            "sample_len": [1],
            "extra_checkpoint_freq": [5],
            "epoch_checkpoint_freq": [1],
            "aux_disc": [True],
            "self_norm": [True],
            "dp_noise_multiplier": [0.01], #, 2.0, 4.0],
            "dp_l2_norm_clip": [1.0]
        }
    ]
}