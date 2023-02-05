This experiment is generated using [MLCommons CM](https://github.com/mlcommons/ck)
## CM Run Command
```
cm run script \
	--tags=run,mlperf,inference,generate-run-cmds,_submission,_full \
	--implementation=nvidia-original \
	--model=bert-99 \
	--backend=tensorrt \
	--device=cuda \
	--execution_mode=valid \
	--push-to-github=on \
	--results_dir=/home/arjun/inference_3.0_results \
	--results_git_url=https://github.com/arjunsuresh/mlperf_inference_submissions_v3.0 \
	--adr.nvidia-harness.skip_preprocess=yes \
	--adr.nvidia-harness.input_format=linear \
	--adr.nvidia-harness.make_cmd=run \
	--env.LD_PRELOAD=/home/arjun/.local/lib/python3.8/site-packages/torch/lib/libgomp-d22c30c5.so.1 \
	--readme=yes
```
## Dependent CM scripts 

`cm run script --tags=detect,os`

`cm run script --tags=detect,cpu`
`cm run script --tags=get,sys-utils-cm`
`cm run script --tags=get,python`
`cm run script --tags=get,cuda`
`cm run script --tags=get,cuda-devices`
`cm run script --tags=get,mlcommons,inference,src,_deeplearningexamples`
`cm run script --tags=get,mlperf,inference,nvidia,common-code`
## Dependent CM scripts for the MLPerf Inference Implementation

`cm run script --tags=detect,os`
`cm run script --tags=detect,cpu`
`cm run script --tags=get,sys-utils-cm`
`cm run script --tags=get,cuda,_cudnn`
`cm run script --tags=get,tensorrt`
`cm run script --tags=build,nvidia,inference,server`
`cm run script --tags=get,mlcommons,inference,src,_deeplearningexamples`
`cm run script --tags=get,nvidia,mlperf,inference,common-code,_custom`
`cm run script --tags=generate,user-conf,mlperf,inference`
