
mouse/ is merged from imgt, ogrdb c57bl, and ogrdb balbc

c57bl/ and balbc/ are just from ogrdb

to update mouse germlines, download from: https://ogrdb.airr-community.org/germline_sets/Mouse
  1) cp unaligned fastas to appropriate dir in ogrdb-downloads/
  2) split apart igh files, cp igk/igl files from germlines/mouse/
  3) run script parse-ogrdb.py from partis main dir
  4) after checking that everything went well, replace old mouse/ dirs with new merged-mouse/ dirs

leader and constant genes from imgt, with extra c genes from the flairr-seq authors
  - Any allele with a name of <gene>_FL_<number> or <gene>*N<number> is novel and not found in the IMGT database.
  - Any allele with the name <gene>-FL or *<number>_ext<number> is an extension of a documented IMGT allele. Some alleles with the first syntax have a letter signifying it is an extension of an IMGT allele but contains unique sequence from other extensions of that allele. 
  - i.e. there's tons of duplicate stuff in here and i'm not sorting through it, whatever
