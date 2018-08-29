FROM yunabe/lgo:latest

WORKDIR /models

RUN go get -u github.com/james-bowman/nlp
RUN go get -u github.com/gocarina/gocsv
RUN go get -u github.com/james-bowman/nlp/measures/pairwise
RUN lgo installpkg github.com/james-bowman/nlp
RUN lgo installpkg github.com/gocarina/gocsv
RUN lgo installpkg github.com/james-bowman/nlp/measures/pairwise
RUN lgo install

CMD ["jupyter", "notebook", "--ip=0.0.0.0"]

