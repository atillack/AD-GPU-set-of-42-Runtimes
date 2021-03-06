# AD-GPU-set-of-42-Runtimes
Runtime tables and dlg files for Diogo's 42 ligand test case on a Titan V

Runs are for collaboration publication and contain sets for the following options:

# Current PR integrating OpenCL and Cuda host code with fixes and same features

All runs used `rand-0.pdbqt` as the ligand and `-lsrat 100.0`. Sequential runs (w/o the filelist option) used the respective `flex-xray.pdbqt` as the xray-ligand for RMSD calculations. Run and Idle times in the results table add up to the overall runtime of a given system. Also, there is a summary at the bottom of each results table.

ADADELTA:

10 runs:
- results.[cuda/opencl].ad.dat
- dlgs/docking-[system]-ad.[cuda/opencl].dlg
- outs/docking-[system-ad.[cuda/opencl].out

Solis-Wets:

10 runs:
- results.[cuda/opencl].sw.dat
- dlgs/docking-[system]-sw.[cuda/opencl].dlg
- outs/docking-[system]-sw.[cuda/opencl].out

10 runs (w/ filelist)
- results.[cuda/opencl].sw.fl.dat
- dlgs/docking-[system]-sw.fl.[cuda/opencl].dlg

100 runs:
- results.[cuda/opencl].sw100.dat
- dlgs/docking-[system]-sw100.[cuda/opencl].dlg
- outs/docking-[system]-sw100.[cuda/opencl].out

100 runs (w/ filelist)
- results.[cuda/opencl].sw100.fl.dat
- dlgs/docking-[system]-sw100.fl.[cuda/opencl].dlg

# "Retro" comparison

Current Cuda fork (Scott Le Grand's relicensing branch at June 10, 2020) and OpenCL (branch from April 3, similar to Cuda in terms of features and fixes). Runs identical to the above.

ADADELTA:

10 runs:
- retro/results.[cuda/opencl].ad.dat
- retro/dlgs/docking-[system]-ad.[cuda/opencl].dlg
- retro/outs/docking-[system-ad.[cuda/opencl].out

Solis-Wets:

10 runs:
- retro/results.[cuda/opencl].sw.dat
- retro/dlgs/docking-[system]-sw.[cuda/opencl].dlg
- retro/outs/docking-[system]-sw.[cuda/opencl].out

100 runs:
- retro/results.[cuda/opencl].sw100.dat
- retro/dlgs/docking-[system]-sw100.[cuda/opencl].dlg
- retro/outs/docking-[system]-sw100.[cuda/opencl].out

