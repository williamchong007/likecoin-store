<!-- eslint-disable max-len -->
<template>
  <div class="home-page v2">
    <header
      class="site-hero"
      :style="`background-image: url(${require('@/assets/webflow/images/hero-bg.jpg')})`"
    >
      <div
        data-collapse="medium"
        data-animation="default"
        data-duration="400"
        data-doc-height="1"
        data-no-scroll="1"
        role="banner"
        class="site-header w-nav"
      >
        <nuxt-link
          class="brand w-nav-brand"
          :to="{ name: 'index' }"
        >
          <img
            loading="lazy"
            src="~/assets/webflow/images/LikeCoin_PressKit_Logo_Fullcolor_Light.svg"
            alt="LikeCoin"
            class="image"
          >
        </nuxt-link>
        <div class="site-menu-wrap">
          <nav
            role="navigation"
            class="site-menu w-nav-menu"
          >
            <a
              href="https://like.co/in/getapp"
              class="site-main-menu__item"
              target="_blank"
            >Download</a>
            <!-- <a
              href="#"
              class="site-main-menu__item"
              target="_blank"
            >Events</a> -->
            <a
              href="https://docs.like.co/user-guide/"
              class="site-main-menu__item"
              target="_blank"
            >User Guide</a>
            <a
              href="https://docs.like.co/developer/"
              class="site-main-menu__item"
              target="_blank"
            >Docs</a>
            <a
              href="https://medium.com/likecoin/"
              class="site-main-menu__item"
              target="_blank"
            >Blog</a>
            <ul
              role="list"
              class="social-media-icons w-list-unstyled"
            >
              <li>
                <a
                  :href="discordURL"
                  target="_blank"
                  class="icon-button-link icon-button-link--dark w-inline-block"
                >
                  <div class="icon-button w-embed">
                    <svg
                      xmlns="http://www.w3.org/2000/svg"
                      viewBox="0 0 204 200"
                      fill="currentColor"
                      width="24px"
                    >
                      <path d="M84,83.9c-5.7,0-10.2,5-10.2,11.1s4.6,11.1,10.2,11.1c5.7,0,10.2-5,10.2-11.1C94.3,88.9,89.7,83.9,84,83.9zM120.5,83.9c-5.7,0-10.2,5-10.2,11.1s4.6,11.1,10.2,11.1c5.7,0,10.2-5,10.2-11.1S126.2,83.9,120.5,83.9z" />
                      <path d="M169.1,0h-134C23.8,0,14.6,9.2,14.6,20.6v135.2c0,11.4,9.2,20.6,20.5,20.6h113.4l-5.3-18.5l12.8,11.9l12.1,11.2l21.5,19V20.6C189.6,9.2,180.4,0,169.1,0z M130.5,130.6c0,0-3.6-4.3-6.6-8.1c13.1-3.7,18.1-11.9,18.1-11.9c-4.1,2.7-8,4.6-11.5,5.9c-5,2.1-9.8,3.5-14.5,4.3c-9.6,1.8-18.4,1.3-25.9-0.1c-5.7-1.1-10.6-2.7-14.7-4.3c-2.3-0.9-4.8-2-7.3-3.4c-0.3-0.2-0.6-0.3-0.9-0.5c-0.2-0.1-0.3-0.2-0.4-0.3c-1.8-1-2.8-1.7-2.8-1.7s4.8,8,17.5,11.8c-3,3.8-6.7,8.3-6.7,8.3c-22.1-0.7-30.5-15.2-30.5-15.2c0-32.2,14.4-58.3,14.4-58.3c14.4-10.8,28.1-10.5,28.1-10.5l1,1.2c-18,5.2-26.3,13.1-26.3,13.1s2.2-1.2,5.9-2.9c10.7-4.7,19.2-6,22.7-6.3c0.6-0.1,1.1-0.2,1.7-0.2c6.1-0.8,13-1,20.2-0.2c9.5,1.1,19.7,3.9,30.1,9.6c0,0-7.9-7.5-24.9-12.7l1.4-1.6c0,0,13.7-0.3,28.1,10.5c0,0,14.4,26.1,14.4,58.3C161.1,115.4,152.6,129.9,130.5,130.6z" />
                    </svg>
                  </div>
                </a>
              </li>
              <li>
                <a
                  href="http://github.com/likecoin"
                  target="_blank"
                  class="icon-button-link icon-button-link--dark w-inline-block"
                >
                  <div class="icon-button w-embed"><svg
                    viewbox="0 0 24 24"
                    xmlns="http://www.w3.org/2000/svg"
                    fill="currentColor"
                  >
                    <path d="m12 .5c-6.63 0-12 5.28-12 11.792 0 5.211 3.438 9.63 8.205 11.188.6.111.82-.254.82-.567 0-.28-.01-1.022-.015-2.005-3.338.711-4.042-1.582-4.042-1.582-.546-1.361-1.335-1.725-1.335-1.725-1.087-.731.084-.716.084-.716 1.205.082 1.838 1.215 1.838 1.215 1.07 1.803 2.809 1.282 3.495.981.108-.763.417-1.282.76-1.577-2.665-.295-5.466-1.309-5.466-5.827 0-1.287.465-2.339 1.235-3.164-.135-.298-.54-1.497.105-3.121 0 0 1.005-.316 3.3 1.209.96-.262 1.98-.392 3-.398 1.02.006 2.04.136 3 .398 2.28-1.525 3.285-1.209 3.285-1.209.645 1.624.24 2.823.12 3.121.765.825 1.23 1.877 1.23 3.164 0 4.53-2.805 5.527-5.475 5.817.42.354.81 1.077.81 2.182 0 1.578-.015 2.846-.015 3.229 0 .309.21.678.825.56 4.801-1.548 8.236-5.97 8.236-11.173 0-6.512-5.373-11.792-12-11.792z" />
                  </svg></div>
                </a>
              </li>
              <li>
                <a
                  href="http://telegram.me/likecoin"
                  target="_blank"
                  class="icon-button-link icon-button-link--dark w-inline-block"
                >
                  <div class="icon-button w-embed"><svg
                    viewbox="0 0 24 24"
                    xmlns="http://www.w3.org/2000/svg"
                    fill="currentColor"
                  >
                    <path d="m9.417 15.181-.397 5.584c.568 0 .814-.244 1.109-.537l2.663-2.545 5.518 4.041c1.012.564 1.725.267 1.998-.931l3.622-16.972.001-.001c.321-1.496-.541-2.081-1.527-1.714l-21.29 8.151c-1.453.564-1.431 1.374-.247 1.741l5.443 1.693 12.643-7.911c.595-.394 1.136-.176.691.218z" />
                  </svg></div>
                </a>
              </li>
              <li>
                <a
                  href="https://twitter.com/likecoin"
                  target="_blank"
                  class="icon-button-link icon-button-link--dark w-inline-block"
                >
                  <div class="icon-button w-embed"><svg
                    xmlns="http://www.w3.org/2000/svg"
                    viewBox="0 0 24 24"
                    fill="currentColor"
                  >
                    <path d="M24,4.56a10.38,10.38,0,0,1-2.84.78,4.94,4.94,0,0,0,2.17-2.72,10.14,10.14,0,0,1-3.12,1.19A4.92,4.92,0,0,0,11.7,7.17a5.07,5.07,0,0,0,.11,1.12A13.94,13.94,0,0,1,1.67,3.15,5,5,0,0,0,1,5.63,4.91,4.91,0,0,0,3.18,9.72,4.81,4.81,0,0,1,1,9.12v.05A5,5,0,0,0,4.9,14a5.36,5.36,0,0,1-1.29.16,4.13,4.13,0,0,1-.93-.09,5,5,0,0,0,4.6,3.43,9.9,9.9,0,0,1-6.1,2.1A9.12,9.12,0,0,1,0,19.54a13.81,13.81,0,0,0,7.55,2.21,13.91,13.91,0,0,0,14-14c0-.22,0-.43,0-.64A9.82,9.82,0,0,0,24,4.56Z" />
                  </svg></div>
                </a>
              </li>
            </ul>
          </nav>
          <a
            class="button button--dark w-button"
            href="https://github.com/sponsors/likecoin"
            target="_blank"
          >Sponsor</a>
          <div class="menu-button w-nav-button">
            <div class="icon w-icon-nav-menu" />
          </div>
        </div>
      </div>
      <div class="site-hero-content">
        <div class="container container--fixed">
          <h1 class="tagline"><strong class="text--bold">Decentralized Publishing Infrastructure.</strong></h1>
          <QuickExchangeWidget
            :api-key="LIQUID_QEX_PUPLIC_API_KEY"
            :wallet-address="walletAddress"
            @success="onQExSuccess"
            @error="onQExError"
          />
        </div>
      </div>
    </header>
    <section class="section">
      <div
        data-w-id="0f837ac9-4bf1-1302-9d48-8f9eaf91ba97"
        style="opacity:0"
        class="container container--fixed"
      >
        <div class="collage">
          <img
            loading="lazy"
            src="~/assets/webflow/images/likecoin-chain.png"
            width="649"
            srcset="~/assets/webflow/images/likecoin-chain-p-500.png 500w, ~/assets/webflow/images/likecoin-chain-p-800.png 800w, ~/assets/webflow/images/likecoin-chain-p-1080.png 1080w, ~/assets/webflow/images/likecoin-chain-p-1600.png 1600w, ~/assets/webflow/images/likecoin-chain-p-2000.png 2000w, ~/assets/webflow/images/likecoin-chain.png 2501w"
            sizes="(max-width: 479px) 92vw, (max-width: 767px) 90vw, (max-width: 991px) 92vw, 42vw"
            alt=""
            class="collage__image collage__image--left"
          >
          <div class="collage__content">
            <h2 class="collage__title collage__title--light">
              <a
                class="link link--light link--no-underline"
                href="https://docs.like.co/validator/likecoin-chain-node"
                target="_blank"
              >LikeCoin chain</a>
            </h2>
            <p class="collage__description">
              Launched in Nov 2019, LikeCoin chain is a public blockchain tailor-made for content publishing. Built on top of Cosmos SDK, it operates under a permissionless, Bonded Proof-of-Stake (BPoS) mechanism. Transactions and data can be browsed on <a
                href="https://likecoin.bigdipper.live"
                class="link link--light"
              >Big Dipper</a> explorer.
              <br>
              <br>
              Join as a validator to help decentralize publishing and earn LikeCoin.
            </p>
            <a
              class="button button--light w-button"
              href="https://docs.like.co/validator/become-a-validator"
              target="_blank"
            >Join as validator</a>
          </div>
        </div>
      </div>
    </section>
    <section class="section section--light section--what-we-do">
      <div class="container container--fixed">
        <h2 class="section__title section__title section__title--light">What LikeCoin Offers</h2>
        <div class="w-layout-grid grid">
          <div class="grid-item">
            <h3 class="grid-item__title">Decentralized Registry</h3>
            <p class="grid-item__content">
              The heart of Decentralized Publishing is decentralized registry powered by <a
                href="https://iscn.io"
                target="_blank"
                class="link link--light"
              >ISCN</a>, a specification we drafted in collaboration with the industry.<br><br>
              Borrowed from the concept of ISBN for books, ISCN is a unique identifier assigned to content such as articles and images, and comes with metadata such as author, publisher, content address, license terms and creation footprint. Stored on LikeCoin chain, ISCN is immutable and censorship resilient. The content, on the other hand, is stored on IPFS for tamper resistance and peer-to-peer distribution.
            </p>
          </div>
          <div class="grid-item">
            <h3 class="grid-item__title">Decentralized Rewards</h3>
            <p class="grid-item__content">By simply attaching a LikeCoin button beneath your content and without setting up a paywall, every Like by readers is turned into measurable rewards in LikeCoin tokens.
              <br>
              <br>
              The <a
                href="https://liker.land/civic"
                class="link link--light"
              >Civic Liker</a> movement encourages readers to contribute USD5/mo to reward creativity and journalism, while the matching fund, distributed according to the Likes of all users, doubles the rewarding pool. With decentralized rewards, every Like counts.</p>
          </div>
          <div class="grid-item">
            <h3 class="grid-item__title">Decentralized Editorial</h3>
            <p class="grid-item__content">Apart from rewarding creators as a Liker, readers may go further to become a Content Jockey.
              <br>
              <br>
              Content Jockeys help distribute creative stories and insightful commentaries with Super Likes, which are purposely designed to be scarce to cut out noise from signals. When a story gets popular, LikeCoin's unique distribution footprint rewards both creator and Content Jockey, creating an all win situation for the content ecosystem.
            </p>
          </div>
          <div class="grid-item">
            <h3 class="grid-item__title">Decentralized Governance</h3>
            <p class="grid-item__content">Not only is LikeCoin token a reward to creators and Content Jockeys, it also serves doubly as the governing token for the decentralized autonomous organization (DAO), namely the Republic of Liker Land.
              <br>
              <br>
              Likers participate in liquid democracy by delegating their LikeCoin tokens to validators they trust, and freely switch among them without a fixed term of office. Issues such as default Content Jockeys, inflation rate and protocol updates require passing a corresponding proposal by the Republic.
            </p>
          </div>
        </div>
      </div>
    </section>
    <section class="section section--dark section--use-case">
      <div class="container container--fixed">
        <div class="w-layout-grid grid">
          <div
            id="w-node-994d7f87d61d-cba99d90"
            class="grid-item grid-item--intro"
          >
            <h2 class="section__title section__title--dark">Use Cases</h2>
            <p class="section__description">LikeCoin is used by various platforms to decentralize publishing and has cultivated a vibrant community. As of August 2020, Republic of Liker Land has <strong class="text--bold">80,076+ Likers</strong>, <strong class="text--bold">289,923+ content</strong> by <strong class="text--bold">11,040+ creators</strong> on <strong class="text--bold">1200+ media</strong>.</p>
          </div>
          <div class="grid-item grid-item--hidden-tablet" />
          <div class="grid-item">
            <div class="grid-item__image-wrapper"><img
              loading="lazy"
              src="~/assets/webflow/images/app.png"
              srcset="~/assets/webflow/images/app-p-500.png 500w, ~/assets/webflow/images/app-p-1080.png 1080w, ~/assets/webflow/images/app.png 1200w"
              sizes="(max-width: 479px) 92vw, (max-width: 767px) 90vw, (max-width: 991px) 92vw, 83vw"
              alt="Liker Land"
              class="grid-item__image"
            ></div>
            <h3 class="grid-item__title grid-item__title--center"><a
              href="https://like.co/in/getapp"
              target="_blank"
              class="link link--dark link--no-underline"
            >Liker Land</a></h3>
            <div class="grid-item__meta">
              <div class="tag">Mobile App</div>
            </div>
            <p class="grid-item__content">Liker Land is a reader, passport, and wallet in one mobile app. Its unique daily content feed is 100% humanly curated by Content Jockyes you trust. With the innovative Super Like feature, Liker Land traces distribution footprint and rewards both Creators and Content Jockeys to cultivate a healthy content ecosystem.</p>
          </div>
          <div class="grid-item">
            <div class="grid-item__image-wrapper"><img
              loading="lazy"
              src="~/assets/webflow/images/browser-extension.jpg"
              srcset="~/assets/webflow/images/browser-extension-p-500.jpeg 500w, ~/assets/webflow/images/browser-extension-p-800.jpeg 800w, ~/assets/webflow/images/browser-extension-p-1080.jpeg 1080w, ~/assets/webflow/images/browser-extension.jpg 1200w"
              sizes="(max-width: 479px) 92vw, (max-width: 767px) 90vw, (max-width: 991px) 92vw, 83vw"
              alt="LikeCoin Browser Extension"
              class="grid-item__image"
            ></div>
            <h3 class="grid-item__title grid-item__title--center"><a
              href="https://chrome.google.com/webstore/detail/liker-land/cjjcemdmkddjbofomfgjedpiifpgkjhe?hl=en"
              target="_blank"
              class="link link--dark link--no-underline"
            >Chrome</a>, <a
              href="https://addons.mozilla.org/en-US/firefox/addon/liker-land/?src=search"
              target="_blank"
              class="link link--dark link--no-underline"
            >Firefox</a>, <a
              href="https://chrome.google.com/webstore/detail/liker-land/cjjcemdmkddjbofomfgjedpiifpgkjhe"
              target="_blank"
              class="link link--dark link--no-underline"
            >Brave</a></h3>
            <div class="grid-item__meta">
              <div class="tag">Browser Extension</div>
            </div>
            <p class="grid-item__content">Liker Land also features an extension for major browsers on computers. Users may save any web page to reading list and access from Liker Land app or <a
              href="https://liker.land/"
              class="link link--dark"
            >website</a> for future reference.<br></p>
          </div>
          <div class="grid-item">
            <div class="grid-item__image-wrapper"><img
              loading="lazy"
              src="~/assets/webflow/images/media-wordpress.svg"
              alt="WordPress"
              class="grid-item__image"
            ></div>
            <h3 class="grid-item__title grid-item__title--center"><a
              href="https://wordpress.org/plugins/likecoin/"
              target="_blank"
              class="link link--dark link--no-underline"
            >WordPress</a></h3>
            <div class="grid-item__meta">
              <div class="tag">Plugin</div>
            </div>
            <p class="grid-item__content">LikeCoin button was first released on WordPress as a plugin in 2018. It allows creators to install and attach to websites and blogs. The button is connected to the LikeCoin reward mechanism and turn each Like into an actual reward. As of May 2020, it has more than 1000 active installations.</p>
          </div>
          <div class="grid-item">
            <div class="grid-item__image-wrapper"><img
              loading="lazy"
              src="~/assets/webflow/images/media-likersocial.svg"
              alt="Liker.Social"
              class="grid-item__image"
            ></div>
            <h3 class="grid-item__title grid-item__title--center"><a
              href="https://liker.social/"
              target="_blank"
              class="link link--dark link--no-underline"
            >Liker.Social</a></h3>
            <div class="grid-item__meta">
              <div class="tag"><strong>Social Media</strong></div>
            </div>
            <p class="grid-item__content">Decentralized microblogs based on LikeCoin & Mastodon open source facilities, supporting likes for rewards, helping creators connect with their own communities and earn revenue from likes and subscriptions.<br></p>
          </div>
          <div class="grid-item">
            <div class="grid-item__image-wrapper"><img
              loading="lazy"
              src="~/assets/webflow/images/media-matters.svg"
              alt="Matters"
              class="grid-item__image"
            ></div>
            <h3 class="grid-item__title grid-item__title--center"><a
              href="https://matters.news/"
              target="_blank"
              class="link link--dark link--no-underline"
            >Matters</a></h3>
            <div class="grid-item__meta">
              <div class="tag"><strong>Public Discussion</strong></div>
            </div>
            <p class="grid-item__content">Matters Lab is a decentralized content platform that provides a shared infrastructure to creators. Matters and LikeCoin developed their partnership since 2018, LikeCoin helps provide an open-source solution to build a decentralized independent journalist network. The partnership is a winning Innovation project of the <a
              href="https://newsinitiative.withgoogle.com/innovation-challenges/funding/"
              class="link link--dark"
            >Google News Initiative 2020</a>.<br></p>
          </div>
          <div class="grid-item">
            <div class="grid-item__image-wrapper"><img
              loading="lazy"
              src="~/assets/webflow/images/media-standnews.svg"
              alt="Stand News"
              class="grid-item__image"
            ></div>
            <h3 class="grid-item__title grid-item__title--center"><a
              href="https://www.thestandnews.com/"
              target="_blank"
              class="link link--dark link--no-underline"
            >Stand News</a></h3>
            <div class="grid-item__meta">
              <div class="tag">Media</div>
            </div>
            <p class="grid-item__content">Stand News is a free not-for-profit online news website based in Hong Kong. It primarily focuses on social and political issues in Hong Kong. It has a monthly 5.4M viewership.</p>
          </div>
          <div class="grid-item">
            <div class="grid-item__image-wrapper"><img
              loading="lazy"
              src="~/assets/webflow/images/media-inmediahk.svg"
              alt="Hong Kong In-media"
              class="grid-item__image"
            ></div>
            <h3 class="grid-item__title grid-item__title--center"><a
              href="https://www.inmediahk.net/"
              target="_blank"
              class="link link--dark link--no-underline"
            >Hong Kong In-media</a></h3>
            <div class="grid-item__meta">
              <div class="tag">Media</div>
            </div>
            <p class="grid-item__content">Hong Kong In-Media is an independent online media platform in Hong Kong. It aims to provide an open public platform for the public and journalists, free from political intervention and commercial influence. It primarily focuses on local news content and opinions. </p>
          </div>
          <div class="grid-item">
            <div class="grid-item__image-wrapper"><img
              loading="lazy"
              src="~/assets/webflow/images/media-hkcnews.svg"
              alt="Hong Kong Citizen News"
              class="grid-item__image"
            ></div>
            <h3 class="grid-item__title grid-item__title--center"><a
              href="https://www.hkcnews.com/"
              target="_blank"
              class="link link--dark link--no-underline"
            >Hong Kong Citizen News</a></h3>
            <div class="grid-item__meta">
              <div class="tag">Media</div>
            </div>
            <p class="grid-item__content">Hong Kong Citizen News is a not-for-profit online news website. It primary focuses on investigative and data-driven journalism to promote fair and neutral new content to the public. <br></p>
          </div>
          <div class="grid-item">
            <div class="grid-item__image-wrapper"><img
              loading="lazy"
              src="~/assets/webflow/images/media-vocus.svg"
              alt="Vocus"
              class="grid-item__image"
            ></div>
            <h3 class="grid-item__title grid-item__title--center"><a
              href="https://vocus.cc/"
              target="_blank"
              class="link link--dark link--no-underline"
            >Vocus</a></h3>
            <div class="grid-item__meta">
              <div class="tag">Blogging Platform</div>
            </div>
            <p class="grid-item__content">Vocus is a new-style content creation platform. It aims to provide a clean and simple reading space with no ads. It also supports multiple content payment mechanisms to readers. It attracts users from Chinese community such as Taiwan and Hong Kong.<br></p>
          </div>
          <div class="grid-item">
            <div class="grid-item__image-wrapper"><img
              loading="lazy"
              src="~/assets/webflow/images/media-medium.svg"
              alt="Medium"
              class="grid-item__image"
            ></div>
            <h3 class="grid-item__title grid-item__title--center"><a
              href="https://medium.com/"
              target="_blank"
              class="link link--dark link--no-underline"
            >Medium</a></h3>
            <div class="grid-item__meta">
              <div class="tag">Plugin</div>
            </div>
            <p class="grid-item__content">LikeCoin plugin also works on Medium and various blogging platforms supporting <a
              href="https://embed.ly/"
              class="link link--dark link--no-underline"
            >embedly</a>. Content creators are able to embed LikeCoin button to their content once registered a Liker ID. No coding required.<br></p>
          </div>
        </div>
        <div class="use-case__footer">
          <a
            href="https://medium.com/likecoin"
            target="_blank"
            class="button button--dark w-button"
          >Follow us on Medium</a>
        </div>
      </div>
    </section>
    <Footer :version="2" />
  </div>
</template>

<script>
import { mapGetters } from 'vuex';

import Footer from '../components/footer/Footer';
import QuickExchangeWidget from '../components/LiquidQuickExchangeWidget/LiquidQuickExchangeWidget';

import {
  DISCORD_INVITE_URL,
  LIQUID_QEX_PUPLIC_API_KEY,
} from '../constant';

import { apiPostLog } from '../util/api/api';

export default {
  name: 'home',
  layout: 'webflow',
  components: {
    Footer,
    QuickExchangeWidget,
  },
  asyncData({ query, redirect }) {
    if (query.press) {
      redirect(302, { name: 'in-about' }, query);
    }
  },
  data() {
    return {
      isWebflowInited: false,
    };
  },
  computed: {
    ...mapGetters([
      'getUserInfo',
    ]),
    LIQUID_QEX_PUPLIC_API_KEY() {
      return LIQUID_QEX_PUPLIC_API_KEY;
    },
    walletAddress() {
      return this.getUserInfo ? this.getUserInfo.cosmosWallet : null;
    },
    discordURL() {
      return DISCORD_INVITE_URL;
    },
  },
  head() {
    return {
      title: this.$t('HomeV2.Meta.Title'),
      meta: [
        {
          hid: 'og_title',
          property: 'og:title',
          content: this.$t('HomeV2.Meta.Og.Title'),
        },
        {
          hid: 'description',
          name: 'description',
          content: this.$t('HomeV2.Meta.Description'),
        },
        {
          hid: 'og_description',
          property: 'og:description',
          content: this.$t('HomeV2.Meta.Og.Description'),
        },
        {
          hid: 'og_image',
          property: 'og:image',
          content: 'https://like.co/images/og/default.png',
        },
      ],
      link: [
        { rel: 'preload', href: 'https://partners.liquid.com/static/liquid-qex-widget/index.umd.js', as: 'script' },
      ],
    };
  },
  mounted() {
    if (window.fbq) window.fbq('track', 'ViewContent');
    if (window.jQuery && window.Webflow) {
      this.initWebflow();
    } else {
      window.Webflow = [];
      window.Webflow.push(() => {
        this.initWebflow();
        window.scrollBy(0, 1);
      });
    }
  },
  methods: {
    initWebflow() {
      if (!window.Webflow) return;
      this.isWebflowInited = true;
      /**
       * ----------------------------------------------------------------------
       * Webflow: Interactions 2.0: Init
       */
      window.Webflow.require('ix2').init(
        {
          events: {
            'e-9': {
              id: 'e-9',
              eventTypeId: 'SCROLL_INTO_VIEW',
              action: {
                id: '', actionTypeId: 'SLIDE_EFFECT', config: { actionListId: 'slideInBottom', autoStopEventId: 'e-10' }, instant: false,
              },
              mediaQueries: ['main', 'medium', 'small', 'tiny'],
              target: { selector: '.grid-item', originalId: '5eb272b2dc812d6acba99d90|15458f6f-954b-d88e-5064-16caab82cf09', appliesTo: 'CLASS' },
              config: {
                loop: false, playInReverse: false, scrollOffsetValue: 10, scrollOffsetUnit: '%', delay: 0, direction: 'BOTTOM', effectIn: true,
              },
              createdOn: 1589251892706,
            },
            'e-23': {
              id: 'e-23',
              eventTypeId: 'SCROLL_INTO_VIEW',
              action: {
                id: '', actionTypeId: 'SLIDE_EFFECT', config: { actionListId: 'slideInBottom', autoStopEventId: 'e-24' }, instant: false,
              },
              mediaQueries: ['main', 'medium', 'small', 'tiny'],
              target: { appliesTo: 'ELEMENT', styleBlockIds: [], id: '5eb272b2dc812d6acba99d90|0f837ac9-4bf1-1302-9d48-8f9eaf91ba97' },
              config: {
                loop: false, playInReverse: false, scrollOffsetValue: 10, scrollOffsetUnit: '%', delay: 0, direction: 'BOTTOM', effectIn: true,
              },
              createdOn: 1589260299658,
            },
            'e-27': {
              id: 'e-27',
              eventTypeId: 'SCROLL_INTO_VIEW',
              action: {
                id: '', actionTypeId: 'FADE_EFFECT', config: { actionListId: 'fadeIn', autoStopEventId: 'e-28' }, instant: false,
              },
              mediaQueries: ['main', 'medium', 'small', 'tiny'],
              target: { selector: '.tagline', originalId: '5eb272b2dc812d6acba99d90|df42c89d-2155-6127-efb7-b0ec5ff8eeb9', appliesTo: 'CLASS' },
              config: {
                loop: false, playInReverse: false, scrollOffsetValue: 10, scrollOffsetUnit: '%', delay: 0, direction: null, effectIn: true,
              },
              createdOn: 1589262452762,
            },
            'e-29': {
              id: 'e-29',
              eventTypeId: 'SCROLL_INTO_VIEW',
              action: {
                id: '', actionTypeId: 'FADE_EFFECT', config: { actionListId: 'fadeIn', autoStopEventId: 'e-30' }, instant: false,
              },
              mediaQueries: ['main', 'medium', 'small', 'tiny'],
              target: { selector: '.container', originalId: '5eb272b2dc812d6acba99d90|0f837ac9-4bf1-1302-9d48-8f9eaf91ba97', appliesTo: 'CLASS' },
              config: {
                loop: false, playInReverse: false, scrollOffsetValue: 10, scrollOffsetUnit: '%', delay: 0, direction: null, effectIn: true,
              },
              createdOn: 1589262546286,
            },
          },
          actionLists: {
            slideInBottom: {
              id: 'slideInBottom',
              useFirstGroupAsInitialState: true,
              actionItemGroups: [{
                actionItems: [{
                  actionTypeId: 'STYLE_OPACITY',
                  config: {
                    delay: 0, duration: 0, target: { id: 'N/A', appliesTo: 'TRIGGER_ELEMENT', useEventTarget: true }, value: 0,
                  },
                }],
              }, {
                actionItems: [{
                  actionTypeId: 'TRANSFORM_MOVE',
                  config: {
                    delay: 0, duration: 0, target: { id: 'N/A', appliesTo: 'TRIGGER_ELEMENT', useEventTarget: true }, xValue: 0, yValue: 100, xUnit: 'PX', yUnit: 'PX', zUnit: 'PX',
                  },
                }],
              }, {
                actionItems: [{
                  actionTypeId: 'TRANSFORM_MOVE',
                  config: {
                    delay: 0, easing: 'outQuart', duration: 1000, target: { id: 'N/A', appliesTo: 'TRIGGER_ELEMENT', useEventTarget: true }, xValue: 0, yValue: 0, xUnit: 'PX', yUnit: 'PX', zUnit: 'PX',
                  },
                }, {
                  actionTypeId: 'STYLE_OPACITY',
                  config: {
                    delay: 0, easing: 'outQuart', duration: 1000, target: { id: 'N/A', appliesTo: 'TRIGGER_ELEMENT', useEventTarget: true }, value: 1,
                  },
                }],
              }],
            },
            fadeIn: {
              id: 'fadeIn',
              useFirstGroupAsInitialState: true,
              actionItemGroups: [{
                actionItems: [{
                  actionTypeId: 'STYLE_OPACITY',
                  config: {
                    delay: 0, duration: 0, target: { id: 'N/A', appliesTo: 'TRIGGER_ELEMENT', useEventTarget: true }, value: 0,
                  },
                }],
              }, {
                actionItems: [{
                  actionTypeId: 'STYLE_OPACITY',
                  config: {
                    delay: 0, easing: 'outQuart', duration: 1000, target: { id: 'N/A', appliesTo: 'TRIGGER_ELEMENT', useEventTarget: true }, value: 1,
                  },
                }],
              }],
            },
          },
          site: { mediaQueries: [{ key: 'main', min: 992, max: 10000 }, { key: 'medium', min: 768, max: 991 }, { key: 'small', min: 480, max: 767 }, { key: 'tiny', min: 0, max: 479 }] },
        },
      );
    },
    onQExSuccess(transaction) {
      try {
        const {
          transaction_id: txId,
          status,
          funding_settlement: {
            transaction_id: fundingTxId,
            currency: fundingCurrency,
            method: fundingMethod,
            quantity: fundingQuantity,
          },
          payout_settlement: {
            transaction_id: payoutTxId,
            currency: payoutCurrency,
            method: payoutMethod,
            quantity: payoutQuantity,
          },
        } = transaction;
        apiPostLog('eventQuickExchange', {
          txId,
          status,
          fundingTxId,
          fundingCurrency,
          fundingMethod,
          fundingQuantity,
          payoutTxId,
          payoutCurrency,
          payoutMethod,
          payoutQuantity,
        });
      } catch (error) {
        // eslint-disable-next-line no-console
        console.error('Quick Exchange Widget Logging Error:', error);
      }
    },
    onQExError(errors) {
      // eslint-disable-next-line no-console
      console.error('Quick Exchange Widget Errors:', errors);
    },
  },
};
</script>

<style lang="scss">
.site-hero-content {
  @media screen and (min-width: 800px) {
    .container {
      display: flex;
      align-items: center;

      h1 {
        flex-grow: 1;

        margin-right: 100px;

        text-align: left;
      }
    }
  }

  @media screen and (max-width: 799px) {
    padding-right: 10px !important;
    padding-left: 10px !important;

    .container {
      padding-right: 0 !important;
      padding-left: 0 !important;
    }

    .liquid-quick-exchange-widget {
      margin: 12px auto 0;
    }
  }
}

@media screen and (min-width: 991px) {
  .section--what-we-do .grid {
    grid-template-columns: 1fr 1fr;
  }
}
</style>
