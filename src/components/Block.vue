<template>
    <section class="block" :style="blockStyles">
        <div class="background" />

        <!-- <BackgroundImage
                Tag="div"
                class="background"
                fluid={desktop.childImageSharp.fluid}
            /> -->
        <div class="block-grid">
            <div
                class="block-grid-item use-m-margin grid__item"
                :style="defaultStyles"
            >
                <div class="text-box block-grid-item__component">
                    <p class="h-3">
                        <span>Text block </span><g-link to="/about">about link</g-link>.
                    </p>
                </div>
            </div>
            <div
                class="block-grid-item use-m-margin grid__item"
                :style="image1Styles"
            >
                <g-image
                    src="~/images/1.JPG"
                    width="294"
                    height="196"
                    alt="alt"
                />
            </div>
            <div
                class="block-grid-item use-m-margin grid__item"
                :style="image2Styles"
            >
                <g-image
                    src="~/images/2.JPG"
                    alt="alt"
                    width="294"
                    height="196"
                />
            </div>
            <div
                class="block-grid-item use-m-margin grid__item"
                :style="image3Styles"
            >
                <g-image
                    src="~/images/3.JPG"
                    width="500"
                    height="334"
                    alt="alt"
                />
            </div>
            <div
                class="block-grid-item use-m-margin grid__item"
                :style="image4Styles"
            >
                <g-image
                    src="~/images/4.JPG"
                    width="604"
                    height="402"
                    alt="alt"
                />
            </div>
            <div
                class="block-grid-item use-m-margin grid__item"
                :style="image5Styles"
            >
                <g-image
                    src="~/images/5.JPG"
                    width="1224"
                    height="816"
                    alt="alt"
                />
            </div>
        </div>
    </section>
</template>

<script>
import moment from "moment";
import * as uuid from "uuid";

const blockStyles = {
    "--rows": 16,
    "--width": "1224px",
    "--m-rows": "9",
    "--row-gap": "16px",
    "--row-size": "64px",
    "--attachment": "unset",
    "--column-gap": "16px",
    "--grid-width": "1224px",
    "--column-count": "12",
    "--block-padding": "10px 0 10px 0",
    "--content-width": "1600px",
    "--content-padding": "16px",
    "--m-block-padding": "64px 16px 56px 16px",
    "--oldContentWidth": "1600px",
    "--grid-gap-history": "16px 24px",
};

const defaultStyles = {
    "--text": "center",
    "--align": "flex-start",
    "--justify": "flex-start",
    "--position": "1/3/2/15",
    "--m-element-margin": "0 0 16px 0",
};

const image1Styles = {
    ...defaultStyles,
    "--position": "2/3/4/6",
};

const image2Styles = {
    ...defaultStyles,
    "--position": "2/6/4/9",
};

const image3Styles = {
    ...defaultStyles,
    "--position": "2/9/6/14",
};

const image4Styles = {
    ...defaultStyles,
    "--position": "4/3/8/9",
};

const image5Styles = {
    ...defaultStyles,
    "--position": "8/3/16/15",
};

export default {
    data: () => ({
        blockStyles,
        defaultStyles,
        image1Styles,
        image2Styles,
        image3Styles,
        image4Styles,
        image5Styles,
    }),
    setup() {
        moment.now();
        uuid.v4();

        return;
    },
};
</script>
