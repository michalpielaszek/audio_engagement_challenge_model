Windows:

cd D:\projekty (tu trzeba podać ścieżkę do folderu z projektami)     
git clone https://github.com/<twoj_login>/<nazwa_repo>.git
cd audio_engagement_challenge_model

Po tym powinny zostać pobrane wszystkie rzeczy związane, z naszą pracą. Następnie trzeba utworzyć wirtualne środowisko conda. Należy upewnić się czy jest plik "environment.yml", na jego bazie odtworzone zostanie środowisko conda.

conda env create -f environment.yml

conda activate wt_model

conda install ipykernel

python -m ipykernel install --user --name wt_model --display-name "Python (wt_model)"

conda list    # to powinno podrzucić informacje na temat zainstalowanych pakietów. Jeśli pokrywa się z environment.yml (wersje dobrze żeby były wyższe o ile jakieś są podane w environment.yml).
