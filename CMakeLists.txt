idf_component_register(
    SRCS
        # Harfbuzz
        "harfbuzz/src/hb-aat-layout.cc"
        "harfbuzz/src/hb-aat-map.cc"
        "harfbuzz/src/hb-blob.cc"
        "harfbuzz/src/hb-buffer.cc"
        "harfbuzz/src/hb-buffer-serialize.cc"
        "harfbuzz/src/hb-buffer-verify.cc"
        "harfbuzz/src/hb-common.cc"
        "harfbuzz/src/hb-draw.cc"
        "harfbuzz/src/hb-font.cc"
        "harfbuzz/src/hb-face.cc"
        "harfbuzz/src/hb-fallback-shape.cc"
        "harfbuzz/src/hb-ft.cc"
        "harfbuzz/src/hb-number.cc"
        "harfbuzz/src/hb-ot-metrics.cc"
        "harfbuzz/src/hb-ot-cff1-table.cc"
        "harfbuzz/src/hb-ot-cff2-table.cc"
        "harfbuzz/src/hb-ot-color.cc"
        "harfbuzz/src/hb-ot-face.cc"
        "harfbuzz/src/hb-ot-font.cc"
        "harfbuzz/src/hb-ot-layout.cc"
        "harfbuzz/src/hb-ot-map.cc"
        "harfbuzz/src/hb-ot-shape.cc"
        "harfbuzz/src/hb-ot-shape-fallback.cc"
        "harfbuzz/src/hb-ot-shape-normalize.cc"
        "harfbuzz/src/hb-ot-shaper-arabic.cc"
        "harfbuzz/src/hb-ot-shaper-default.cc"
        "harfbuzz/src/hb-ot-shaper-hangul.cc"
        "harfbuzz/src/hb-ot-shaper-hebrew.cc"
        "harfbuzz/src/hb-ot-shaper-indic-table.cc"
        "harfbuzz/src/hb-ot-shaper-indic.cc"
        "harfbuzz/src/hb-ot-shaper-khmer.cc"
        "harfbuzz/src/hb-ot-shaper-myanmar.cc"
        "harfbuzz/src/hb-ot-shaper-syllabic.cc"
        "harfbuzz/src/hb-ot-shaper-thai.cc"
        "harfbuzz/src/hb-ot-shaper-use.cc"
        "harfbuzz/src/hb-ot-shaper-vowel-constraints.cc"
        "harfbuzz/src/hb-ot-tag.cc"
        "harfbuzz/src/hb-ot-var.cc"
        "harfbuzz/src/hb-outline.cc"
        "harfbuzz/src/hb-paint.cc"
        "harfbuzz/src/hb-paint-extents.cc"
        "harfbuzz/src/hb-shape.cc"
        "harfbuzz/src/hb-shape-plan.cc"
        "harfbuzz/src/hb-shaper.cc"
        "harfbuzz/src/hb-static.cc"
        "harfbuzz/src/hb-ucd.cc"
        "harfbuzz/src/hb-unicode.cc"


    INCLUDE_DIRS
        "harfbuzz/src"

    REQUIRES
        espressif__freetype
)

# Add compile definitions
target_compile_definitions(${COMPONENT_LIB} PRIVATE
    -DHAVE_FREETYPE=1
)


