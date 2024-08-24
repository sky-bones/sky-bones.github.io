# liz nichols portfolio website
--
Hello. Here are some notes about the files above.

1. index.html is the main site code. it has all the website text and image files and basic HTML structure. most website hosting sites will recognize index.html as the main / home page of a site and will by default render it at the root domain

2. site.css and static.css are stripped from squarespace and just saved locally so there's no more style dependency. they are minified and ugly and i recommend just leaving them as they are.

3. thenewstuff.css is my new CSS file with my own custom styles. this was needed to replicate mainly to replicate the image grid experience outside of squarespace. i cut any JS dependencies and without them, the grid kinda crashed. this thenewstuff.css fixes it back up again. this is the file we'll edit if new styles are needed on site. 

4. site-bundles.js is actually unneeded. it's here when i tried stripping the JS files to render locally, but it didn't work. and honestly it just isn't needed. your site doesn't require JS right now, and if it does in the future, we'll just start from scratch.

--

Here are the HTML snippets for the GALLERY sections. There are three snippet options. One-column, two-column, and three-column. They are listed below.

### Two Column
    <section
        data-test="page-section"
        data-section-theme=""
        class="page-section gallery-section full-bleed-section background-width--full-bleed section-height--medium content-width--wide horizontal-alignment--center vertical-alignment--middle"
        data-section-id="twocolumn"
        data-controller="SectionWrapperController"
        data-animation="none"
        data-json-schema-section
    >
        <div class="section-border">
            <div class="section-background"></div>
        </div>
        <div class="content-wrapper" style="">
            <div class="content">
                <div class="gallery gallery-section-wrapper" style="min-height: 100px;">
                    <div class="gallery" style="min-height: 100px;">
                        <!-- Gallery Grid -->
                        <div
                            class="gallery-grid gallery-grid--layout-grid"
                            data-controller="GalleryGrid"
                            data-section-id="twocolumn"
                            data-animation="site-default"
                            data-lightbox=""
                            data-width="full"
                            data-aspect-ratio="square"
                            data-columns="2"
                            data-gutter="75"
                            data-props='{"aspectRatio": "square","scrollAnimation": "site-default","gutter": 75,"numColumns": 2,"width": "full","lightboxEnabled": false}'
                            data-show-captions="false"
                            data-test="gallery-grid-simple"
                        >
                            <div class="gallery-grid-wrapper">
                                <figure class="gallery-grid-item">
                                    <div class="gallery-grid-item-wrapper" data-animation-role="image">
                                        <img
                                            data-src="img/spc_brand_guide_spread_1.jpg"
                                            data-image="img/spc_brand_guide_spread_1.jpg"
                                            data-image-dimensions="2500x1875"
                                            data-image-focal-point="0.5,0.5"
                                            alt="Spectrum Therapeutics Brand Guide"
                                            data-load="false"
                                            src="img/spc_brand_guide_spread_1.jpg"
                                            width="2500"
                                            height="1875"
                                            alt=""
                                            sizes="64.16666666666666vw"
                                            style="display: block; object-position: 50% 50%; object-fit: cover; width: 100%; height: 100%;"
                                            loading="lazy"
                                            decoding="async"
                                            data-loader="sqs"
                                        />
                                    </div>
                                </figure>
                                <figure class="gallery-grid-item">
                                    <div class="gallery-grid-item-wrapper" data-animation-role="image">
                                        <img
                                            data-src="img/poster_mockup_v2.jpg"
                                            data-image="img/poster_mockup_v2.jpg"
                                            data-image-dimensions="2500x1875"
                                            data-image-focal-point="0.5,0.5"
                                            alt="Clinic Poster"
                                            data-load="false"
                                            src="img/poster_mockup_v2.jpg"
                                            width="2500"
                                            height="1875"
                                            alt=""
                                            sizes="64.16666666666666vw"
                                            style="display: block; object-position: 50% 50%; object-fit: cover; width: 100%; height: 100%;"
                                            loading="lazy"
                                            decoding="async"
                                            data-loader="sqs"
                                        />
                                    </div>
                                </figure>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

### One Column
    <section
        data-test="page-section"
        data-section-theme=""
        class="page-section gallery-section full-bleed-section background-width--full-bleed section-height--medium content-width--wide horizontal-alignment--center vertical-alignment--middle"
        data-section-id="onecolumn"
        data-controller="SectionWrapperController"
        data-animation="none"
        data-json-schema-section
    >
        <div class="section-border">
            <div class="section-background"></div>
        </div>
        <div class="content-wrapper" style="">
            <div class="content">
                <div class="gallery gallery-section-wrapper" style="min-height: 100px;">
                    <div class="gallery" style="min-height: 100px;">
                        <!-- Gallery Grid -->
                        <div
                            class="gallery-grid gallery-grid--layout-grid"
                            data-controller="GalleryGrid"
                            data-section-id="onecolumn"
                            data-animation="site-default"
                            data-lightbox=""
                            data-width="full"
                            data-aspect-ratio="anamorphic-widescreen"
                            data-columns="1"
                            data-gutter="29"
                            data-props='{"aspectRatio": "anamorphic-widescreen","scrollAnimation": "site-default","gutter": 29,"numColumns": 1,"width": "full","lightboxEnabled": false}'
                            data-show-captions="false"
                            data-test="gallery-grid-simple"
                        >
                            <div class="gallery-grid-wrapper">
                                <figure class="gallery-grid-item">
                                    <div class="gallery-grid-item-wrapper" data-animation-role="image">
                                        <img
                                            data-src="img/website_mockup_grid.jpg"
                                            data-image="img/website_mockup_grid.jpg"
                                            data-image-dimensions="2500x1875"
                                            data-image-focal-point="0.5,0.5"
                                            alt="website_mockup_grid copy.jpg"
                                            data-load="false"
                                            src="img/website_mockup_grid.jpg"
                                            width="2500"
                                            height="1875"
                                            alt=""
                                            sizes="100vw"
                                            style="display: block; object-position: 50% 50%; object-fit: cover; width: 100%; height: 100%;"
                                            loading="lazy"
                                            decoding="async"
                                            data-loader="sqs"
                                        />
                                    </div>
                                </figure>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

### Three Column
    <section
        data-test="page-section"
        data-section-theme=""
        class="page-section gallery-section full-bleed-section background-width--full-bleed section-height--medium content-width--wide horizontal-alignment--center vertical-alignment--middle"
        data-section-id="threecolumn"
        data-controller="SectionWrapperController"
        data-animation="none"
        data-json-schema-section
    >
        <div class="section-border">
            <div class="section-background"></div>
        </div>
        <div class="content-wrapper" style="">
            <div class="content">
                <div class="gallery gallery-section-wrapper" style="min-height: 100px;">
                    <div class="gallery" style="min-height: 100px;">
                        <!-- Gallery Grid -->
                        <div
                            class="gallery-grid gallery-grid--layout-grid"
                            data-controller="GalleryGrid"
                            data-section-id="threecolumn"
                            data-animation="site-default"
                            data-lightbox=""
                            data-width="full"
                            data-aspect-ratio="square"
                            data-columns="3"
                            data-gutter="50"
                            data-props='{"aspectRatio": "square","scrollAnimation": "site-default","gutter": 50,"numColumns": 3,"width": "full","lightboxEnabled": false}'
                            data-show-captions="false"
                            data-test="gallery-grid-simple"
                        >
                            <div class="gallery-grid-wrapper">
                                <figure class="gallery-grid-item">
                                    <div class="gallery-grid-item-wrapper" data-animation-role="image">
                                        <img
                                            data-src="img/Choclate-Houndstooth.jpg"
                                            data-image="img/Choclate-Houndstooth.jpg"
                                            data-image-dimensions="520x520"
                                            data-image-focal-point="0.5,0.5"
                                            alt="Choclate-Houndstooth.jpg"
                                            data-load="false"
                                            src="img/Choclate-Houndstooth.jpg"
                                            width="520"
                                            height="520"
                                            alt=""
                                            sizes="(max-width:768px)48.75vw,31.666666666666668vw"
                                            style="display: block; object-position: 50% 50%; object-fit: cover; width: 100%; height: 100%;"
                                            loading="lazy"
                                            decoding="async"
                                            data-loader="sqs"
                                        />
                                    </div>
                                </figure>
                                <figure class="gallery-grid-item">
                                    <div class="gallery-grid-item-wrapper" data-animation-role="image">
                                        <img
                                            data-src="img/Chocolate-Bakerstreet.jpg"
                                            data-image="img/Chocolate-Bakerstreet.jpg"
                                            data-image-dimensions="520x522"
                                            data-image-focal-point="0.5,0.5"
                                            alt="Chocolate-Bakerstreet.jpg"
                                            data-load="false"
                                            src="img/Chocolate-Bakerstreet.jpg"
                                            width="520"
                                            height="522"
                                            alt=""
                                            sizes="(max-width:768px)48.75vw,31.666666666666668vw"
                                            style="display: block; object-position: 50% 50%; object-fit: cover; width: 100%; height: 100%;"
                                            loading="lazy"
                                            decoding="async"
                                            data-loader="sqs"
                                        />
                                    </div>
                                </figure>
                                <figure class="gallery-grid-item">
                                    <div class="gallery-grid-item-wrapper" data-animation-role="image">
                                        <img
                                            data-src="img/Chocolate-Penelope.jpg"
                                            data-image="img/Chocolate-Penelope.jpg"
                                            data-image-dimensions="520x522"
                                            data-image-focal-point="0.5,0.5"
                                            alt="Chocolate-Penelope.jpg"
                                            data-load="false"
                                            src="img/Chocolate-Penelope.jpg"
                                            width="520"
                                            height="522"
                                            alt=""
                                            sizes="(max-width:768px)48.75vw,31.666666666666668vw"
                                            style="display: block; object-position: 50% 50%; object-fit: cover; width: 100%; height: 100%;"
                                            loading="lazy"
                                            decoding="async"
                                            data-loader="sqs"
                                        />
                                    </div>
                                </figure>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>