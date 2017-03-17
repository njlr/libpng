include_defs('//BUCKAROO_DEPS')

cxx_library(
  name = 'libpng',
  header_namespace = '',
  exported_headers = [
    'png.h',
    'pngconf.h',
  ],
  # headers = subdir_glob([
  #   ('', '*.h'),
  # ]),
  srcs = [
    'png.c',
    'pngerror.c',
    'pngget.c',
    'pngmem.c',
    'pngpread.c',
    'pngread.c',
    'pngrio.c',
    'pngrtran.c',
    'pngrutil.c',
    'pngset.c',
    'pngtrans.c',
    'pngwio.c',
    'pngwrite.c',
    'pngwtran.c',
    'pngwutil.c',
  ],
  visibility = [
    'PUBLIC',
  ],
  deps = BUCKAROO_DEPS,
)

cxx_binary(
  name = 'test',
  srcs = [
    'pngtest.c',
  ],
  deps = [
    ':libpng',
  ],
)
