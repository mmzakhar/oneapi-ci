# SPDX-FileCopyrightText: 2020 Intel Corporation
#
# SPDX-License-Identifier: MIT

CXX          = icc
CPP_SAMPLE   = hello

${CPP_SAMPLE}.out: ${CPP_SAMPLE}.bin
	./${CPP_SAMPLE}.bin > $@
	cat $@

${CPP_SAMPLE}.bin: ${CPP_SAMPLE}.cpp
	${CXX} -o $@ $^

clean:
	rm -rf *.out *.bin
