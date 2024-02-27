# acad_workshop202
#Commands for workshop Day 2 
    1  mkdir bin && cd bin/
    2  wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
    3  bash Miniconda3-latest-Linux-x86_64.sh Miniconda3-latest-Linux-x86_64.sh Miniconda3-latest-Linux-x86_64.sh Miniconda3-latest-Linux-x86_64.sh Miniconda3-latest-Linux-x86_64.sh
    4  ls
    5  source ~/.bashrc
    6  conda config --set auto_activate_base false
    7  conda --version
    8  conda config --add channels defaults
    9  conda config --add channels bioconda
   10  conda config --add channels conda-forge
   11  conda create -n nf-core-dsll -c bioconda nextflow=22.10.6
   12  conda activate nf-core-dsl1
   13  conda activate nf-nf-core-dsl1
   14  conda activate nf-core-dsl1
   15  conda env list
   16  nf-core-dsll
   17  conda activate nf-core-dsll
   18  conda deactivate
   19  conda create -n nf-core-dsl2 -c bioconda nextflow=23.10
   20  conda deactivate
   21  spack load apptainer
   22  apptainer --version
   23  singularity --version
   24  cd $HOME
   25  mkdir acad-workshop
   26  ll
   27  cd acad-workshop/
   28  conda activate nf-core-dsl1
   29  conda activate nf-core-dsll
   30  nextflow pull nf-core/eager
   31  nextflow pull nf-core/eager -r 2.5.0
   32  nextflow run nf-core/eager -r 2.5.0. -profile singularity, test --outdir ./test-example
   33  nextflow run nf-core/eager -r 2.5.0 -profile singularity,test --outdir ./test-example
   34  ls
   35  cd ./test-example/
   36  ls
   37  cat .nextflow.log
   38  cd ../
   39  ll
   40  cat .nextflow.log
   41  screen -R Scrn
   42  screen -R Scrn
   43  squeue
   44  ls
   45  cd ./acad-workshop/
   46  ls
   47  cd eager-screening/multiqc/
   48  pwd
   49  nextflow clean -n
   50  conda activate nf-core-dsll
   51  nextflow clean -n
   52  cd ./acad-workshop/
   53  nextflow clean -n
   54  nextflow clean -f
   55  htop
   56  get clone --help
   57  git clone --help
   58  cd acad-workshop
   59  git clone --help
   60  git clone https://github.com/vishwadeeprout/acad_workshop202.git
   61  ls
   62  cd acad_workshop202/
   63  ls
   64  ls -l
   65  vim README.md
   66  git add .
   67  git commit -c "Added my name to header"
   68  git commit -m "Added my name to header"
   69  git config --global user.email "vishwadeep.rout@utas.edu.au
   70  git config --global user.email "vishwadeep.rout@utas.edu.au"
   71  git config --global user.name "vishwadeep.rout"
   72  git commit -m "Added my name to header"
   73  vim README.md
   74  git add .
   75  git commit -m "Added my name to header"
   76  git push
   77  ls
   78  git log
   79  vim .condarc
   80  srun --export=ALL --ntasks-per-node 4 --nodes 1 --mem 40G  -t 01:00:00 --pty bash
   81  srun --export=ALL --ntasks-per-node 4 --nodes 1 --mem 10G  -t 01:00:00 --pty bash
   82  conda deactivate
   83  conda create -n bam-fliter bam-filter
   84  conda create -n bam-fliter
   85  conda create -n bam-filter
   86  conda activate bam-filter
   87  conda install -c conda-forge -c bioconda -c genomewalker bam-filter
   88  conda activate acad-euks_1
   89  ls
   90  mkdir euks
   91  cd euks/
   92  ll
   93  ln -s /shared/data/euks_data/*
   94  ll
   95  conda activate acad-euks_srun -n 1 --mem 1GB  vsearch --fastx_uniques ERR10493277_small-FINAL.fq.gz --fastqout ./ERR10493277_small-FINAL.vs.fq --minseqlength 30 --strand both
   97  ll
   98  exit
   99  screen -Rinstall
  100  screen -R install


