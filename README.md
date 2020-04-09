# Template customization


## src
I hope you have seen this template `src` folder on the downloaded package `Sapp - Angular 9 App Landing Page` from ThemeForest.

In this `src` folder you can see `index.html` file. This file structure is like this-

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <!--meta, title, base, google fonts, all css linking here-->
</head>

<body>

  <app-root></app-root>
 
 <!--all js linking here-->
</body>

</html>
```

All HTML content will be load into this `app-root`:
```html
<app-root></app-root>
```


## entry points

##### app-component.html
Template `app-component.html` structure looks like this-
```html
<router-outlet></router-outlet>

```

##### app-component.ts
Here we have generated all of our components. Template `app-component.ts` structure looks like this-
```js
import { Component } from '@angular/core';

@Component({
  selector: 'app-root',
  templateUrl: './app.component.html',
  styleUrls: ['./app.component.css']
})
export class AppComponent {
  title = 'sapp';
}

```

##### app.module.ts
Template `app.module.ts` structure looks like this-
```js
import { BrowserModule } from '@angular/platform-browser';
import { NgModule } from '@angular/core';

import { AppRoutingModule } from './app-routing.module';
import { AppComponent } from './app.component';
import { WelcomeOneComponent } from './components/welcome/welcome-one/welcome-one.component';
import { CounterComponent } from './components/counter/counter.component';
import { FeatureOneComponent } from './components/features/feature-one/feature-one.component';
import { ServiceOneComponent } from './components/services/service-one/service-one.component';
import { DiscoverOneComponent } from './components/discover/discover-one/discover-one.component';
import { WorkComponent } from './components/work/work.component';
import { ScreenshotOneComponent } from './components/screenshots/screenshot-one/screenshot-one.component';
import { PricingOneComponent } from './components/pricing/pricing-one/pricing-one.component';
import { FaqOneComponent } from './components/faq/faq-one/faq-one.component';
import { TeamComponent } from './components/team/team.component';
import { DownloadComponent } from './components/download/download.component';
import { SubscribeComponent } from './components/subscribe/subscribe.component';
import { ContactComponent } from './components/contact/contact.component';
import { FooterOneComponent } from './components/footer/footer-one/footer-one.component';
import { FooterTwoComponent } from './components/footer/footer-two/footer-two.component';
import { ScrollupComponent } from './components/scrollup/scrollup.component';
import { ThemeOneComponent } from './themes/theme-one/theme-one.component';
import { ThemeTwoComponent } from './themes/theme-two/theme-two.component';
import { WelcomeTwoComponent } from './components/welcome/welcome-two/welcome-two.component';
import { FeatureTwoComponent } from './components/features/feature-two/feature-two.component';
import { DiscoverTwoComponent } from './components/discover/discover-two/discover-two.component';
import { ServiceTwoComponent } from './components/services/service-two/service-two.component';
import { ScreenshotTwoComponent } from './components/screenshots/screenshot-two/screenshot-two.component';
import { ReviewOneComponent } from './components/reviews/review-one/review-one.component';
import { ReviewTwoComponent } from './components/reviews/review-two/review-two.component';
import { FaqTwoComponent } from './components/faq/faq-two/faq-two.component';
import { ThemeThreeComponent } from './themes/theme-three/theme-three.component';
import { ThemeFourComponent } from './themes/theme-four/theme-four.component';
import { ThemeFiveComponent } from './themes/theme-five/theme-five.component';
import { ThemeSixComponent } from './themes/theme-six/theme-six.component';
import { WelcomeThreeComponent } from './components/welcome/welcome-three/welcome-three.component';
import { WelcomeFourComponent } from './components/welcome/welcome-four/welcome-four.component';
import { WelcomeFiveComponent } from './components/welcome/welcome-five/welcome-five.component';
import { WelcomeSixComponent } from './components/welcome/welcome-six/welcome-six.component';
import { FeatureThreeComponent } from './components/features/feature-three/feature-three.component';
import { DiscoverThreeComponent } from './components/discover/discover-three/discover-three.component';
import { ServiceThreeComponent } from './components/services/service-three/service-three.component';
import { ReviewThreeComponent } from './components/reviews/review-three/review-three.component';
import { PricingTwoComponent } from './components/pricing/pricing-two/pricing-two.component';
import { ServiceFourComponent } from './components/services/service-four/service-four.component';
import { DiscoverFourComponent } from './components/discover/discover-four/discover-four.component';
import { FeatureFourComponent } from './components/features/feature-four/feature-four.component';
import { FeatureFiveComponent } from './components/features/feature-five/feature-five.component';
import { ServiceFiveComponent } from './components/services/service-five/service-five.component';
import { DiscoverFiveComponent } from './components/discover/discover-five/discover-five.component';
import { PricingThreeComponent } from './components/pricing/pricing-three/pricing-three.component';
import { ServiceSixComponent } from './components/services/service-six/service-six.component';
import { DiscoverSixComponent } from './components/discover/discover-six/discover-six.component';
import { BrandComponent } from './components/brand/brand.component';
import { FeatureSixComponent } from './components/features/feature-six/feature-six.component';
import { PricingFourComponent } from './components/pricing/pricing-four/pricing-four.component';
import { BlogTwoColumnComponent } from './components/blogs/blog-two-column/blog-two-column.component';
import { BlogThreeColumnComponent } from './components/blogs/blog-three-column/blog-three-column.component';
import { BlogLeftSidebarComponent } from './components/blogs/blog-left-sidebar/blog-left-sidebar.component';
import { BlogRightSidebarComponent } from './components/blogs/blog-right-sidebar/blog-right-sidebar.component';
import { BlogDetailsLeftSidebarComponent } from './components/blogs/blog-details-left-sidebar/blog-details-left-sidebar.component';
import { BlogDetailsRightSidebarComponent } from './components/blogs/blog-details-right-sidebar/blog-details-right-sidebar.component';
import { PricingComponent } from './components/inner-pages/pricing/pricing.component';
import { ThankYouComponent } from './components/inner-pages/thank-you/thank-you.component';
import { ComingSoonComponent } from './components/inner-pages/coming-soon/coming-soon.component';
import { ErrorComponent } from './components/inner-pages/error/error.component';
import { LoginComponent } from './components/accounts/login/login.component';
import { SignupComponent } from './components/accounts/signup/signup.component';
import { ResetComponent } from './components/accounts/reset/reset.component';
import { BreadcrumbPricingComponent } from './components/breadcrumb/breadcrumb-pricing/breadcrumb-pricing.component';
import { BreadcrumbBlogTwoColumnComponent } from './components/breadcrumb/breadcrumb-blog-two-column/breadcrumb-blog-two-column.component';
import { BreadcrumbBlogThreeColumnComponent } from './components/breadcrumb/breadcrumb-blog-three-column/breadcrumb-blog-three-column.component';
import { BreadcrumbBlogLeftSidebarComponent } from './components/breadcrumb/breadcrumb-blog-left-sidebar/breadcrumb-blog-left-sidebar.component';
import { BreadcrumbBlogRightSidebarComponent } from './components/breadcrumb/breadcrumb-blog-right-sidebar/breadcrumb-blog-right-sidebar.component';
import { BreadcrumbBlogDetailsLeftSidebarComponent } from './components/breadcrumb/breadcrumb-blog-details-left-sidebar/breadcrumb-blog-details-left-sidebar.component';
import { BreadcrumbBlogDetailsRightSidebarComponent } from './components/breadcrumb/breadcrumb-blog-details-right-sidebar/breadcrumb-blog-details-right-sidebar.component';
import { BreadcrumbReviewsComponent } from './components/breadcrumb/breadcrumb-reviews/breadcrumb-reviews.component';
import { FaqThreeComponent } from './components/faq/faq-three/faq-three.component';
import { BreadcrumbFaqComponent } from './components/breadcrumb/breadcrumb-faq/breadcrumb-faq.component';
import { BreadcrumbContactComponent } from './components/breadcrumb/breadcrumb-contact/breadcrumb-contact.component';
import { ReviewPageComponent } from './components/inner-pages/review-page/review-page.component';
import { DownloadPageComponent } from './components/inner-pages/download-page/download-page.component';
import { SubscribePageComponent } from './components/inner-pages/subscribe-page/subscribe-page.component';
import { FaqPageComponent } from './components/inner-pages/faq-page/faq-page.component';
import { ContactPageComponent } from './components/inner-pages/contact-page/contact-page.component';
import { HeaderOneComponent } from './components/header/header-one/header-one.component';
import { HeaderTwoComponent } from './components/header/header-two/header-two.component';

@NgModule({
  declarations: [
    AppComponent,
    WelcomeOneComponent,
    CounterComponent,
    FeatureOneComponent,
    ServiceOneComponent,
    DiscoverOneComponent,
    WorkComponent,
    ScreenshotOneComponent,
    PricingOneComponent,
    FaqOneComponent,
    TeamComponent,
    DownloadComponent,
    SubscribeComponent,
    ContactComponent,
    FooterOneComponent,
    FooterTwoComponent,
    ScrollupComponent,
    ThemeOneComponent,
    ThemeTwoComponent,
    WelcomeTwoComponent,
    FeatureTwoComponent,
    DiscoverTwoComponent,
    ServiceTwoComponent,
    ScreenshotTwoComponent,
    ReviewOneComponent,
    ReviewTwoComponent,
    FaqTwoComponent,
    ThemeThreeComponent,
    ThemeFourComponent,
    ThemeFiveComponent,
    ThemeSixComponent,
    WelcomeThreeComponent,
    WelcomeFourComponent,
    WelcomeFiveComponent,
    WelcomeSixComponent,
    FeatureThreeComponent,
    DiscoverThreeComponent,
    ServiceThreeComponent,
    ReviewThreeComponent,
    PricingTwoComponent,
    ServiceFourComponent,
    DiscoverFourComponent,
    FeatureFourComponent,
    FeatureFiveComponent,
    ServiceFiveComponent,
    DiscoverFiveComponent,
    PricingThreeComponent,
    ServiceSixComponent,
    DiscoverSixComponent,
    BrandComponent,
    FeatureSixComponent,
    PricingFourComponent,
    BlogTwoColumnComponent,
    BlogThreeColumnComponent,
    BlogLeftSidebarComponent,
    BlogRightSidebarComponent,
    BlogDetailsLeftSidebarComponent,
    BlogDetailsRightSidebarComponent,
    PricingComponent,
    ThankYouComponent,
    ComingSoonComponent,
    ErrorComponent,
    LoginComponent,
    SignupComponent,
    ResetComponent,
    BreadcrumbPricingComponent,
    BreadcrumbBlogTwoColumnComponent,
    BreadcrumbBlogThreeColumnComponent,
    BreadcrumbBlogLeftSidebarComponent,
    BreadcrumbBlogRightSidebarComponent,
    BreadcrumbBlogDetailsLeftSidebarComponent,
    BreadcrumbBlogDetailsRightSidebarComponent,
    BreadcrumbReviewsComponent,
    FaqThreeComponent,
    BreadcrumbFaqComponent,
    BreadcrumbContactComponent,
    ReviewPageComponent,
    DownloadPageComponent,
    SubscribePageComponent,
    FaqPageComponent,
    ContactPageComponent,
    HeaderOneComponent,
    HeaderTwoComponent,
  ],
  imports: [
    BrowserModule,
    AppRoutingModule
  ],
  providers: [],
  bootstrap: [AppComponent]
})
export class AppModule { }

```


## themes

`themes` folder included on `app` folder. You can check our folder structure on `app` folder menu.
This is `themes` folder structure-
```text
|-- themes
    |-- theme-one ( default theme)
    |-- theme-two ( demo theme 2)
    .....
    |-- theme-six ( demo theme 6 )
```

`themes` folder contains all of our 6 demos.


## app-routing
In `app` folder we used `app-routing.module.ts`. Where we linked all the route for our all theme. For routing we used angular-router.

Routes: `src/app/app-routing.module.ts`

```js
import { NgModule } from '@angular/core';
import { Routes, RouterModule } from '@angular/router';
import { ThemeOneComponent } from './themes/theme-one/theme-one.component';
import { ThemeTwoComponent } from './themes/theme-two/theme-two.component';
import { ThemeThreeComponent } from './themes/theme-three/theme-three.component';
import { ThemeFourComponent } from './themes/theme-four/theme-four.component';
import { ThemeFiveComponent } from './themes/theme-five/theme-five.component';
import { ThemeSixComponent } from './themes/theme-six/theme-six.component';
import { PricingComponent } from './components/inner-pages/pricing/pricing.component';
import { DownloadPageComponent } from './components/inner-pages/download-page/download-page.component';
import { SubscribePageComponent } from './components/inner-pages/subscribe-page/subscribe-page.component';
import { ThankYouComponent } from './components/inner-pages/thank-you/thank-you.component';
import { ComingSoonComponent } from './components/inner-pages/coming-soon/coming-soon.component';
import { ErrorComponent } from './components/inner-pages/error/error.component';
import { BlogTwoColumnComponent } from './components/blogs/blog-two-column/blog-two-column.component';
import { BlogThreeColumnComponent } from './components/blogs/blog-three-column/blog-three-column.component';
import { BlogLeftSidebarComponent } from './components/blogs/blog-left-sidebar/blog-left-sidebar.component';
import { BlogRightSidebarComponent } from './components/blogs/blog-right-sidebar/blog-right-sidebar.component';
import { BlogDetailsLeftSidebarComponent } from './components/blogs/blog-details-left-sidebar/blog-details-left-sidebar.component';
import { BlogDetailsRightSidebarComponent } from './components/blogs/blog-details-right-sidebar/blog-details-right-sidebar.component';
import { LoginComponent } from './components/accounts/login/login.component';
import { SignupComponent } from './components/accounts/signup/signup.component';
import { ResetComponent } from './components/accounts/reset/reset.component';
import { ReviewPageComponent } from './components/inner-pages/review-page/review-page.component';
import { FaqPageComponent } from './components/inner-pages/faq-page/faq-page.component';
import { ContactPageComponent } from './components/inner-pages/contact-page/contact-page.component';

const routes: Routes = [
  {path: '', component: ThemeOneComponent},
  {path: 'theme-two', component: ThemeTwoComponent},
  {path: 'theme-three', component: ThemeThreeComponent},
  {path: 'theme-four', component: ThemeFourComponent},
  {path: 'theme-five', component: ThemeFiveComponent},
  {path: 'theme-six', component: ThemeSixComponent},
  {path: 'pricing', component: PricingComponent},
  {path: 'download', component: DownloadPageComponent},
  {path: 'subscribe', component: SubscribePageComponent},
  {path: 'thank-you', component: ThankYouComponent},
  {path: 'coming-soon', component: ComingSoonComponent},
  {path: 'error', component: ErrorComponent},
  {path: 'blog-two-column', component: BlogTwoColumnComponent},
  {path: 'blog-three-column', component: BlogThreeColumnComponent},
  {path: 'blog-left-sidebar', component: BlogLeftSidebarComponent},
  {path: 'blog-right-sidebar', component: BlogRightSidebarComponent},
  {path: 'blog-details-left-sidebar', component: BlogDetailsLeftSidebarComponent},
  {path: 'blog-details-right-sidebar', component: BlogDetailsRightSidebarComponent},
  {path: 'login', component: LoginComponent},
  {path: 'signup', component: SignupComponent},
  {path: 'reset', component: ResetComponent},
  {path: 'reviews', component: ReviewPageComponent},
  {path: 'faq', component: FaqPageComponent},
  {path: 'contact', component: ContactPageComponent}
];

@NgModule({
  imports: [RouterModule.forRoot(routes)],
  exports: [RouterModule]
})
export class AppRoutingModule { }

```


## components
Under `components` folder we generated all of our components individually. 
We have generated these components to make the developer’s life easy. 
By using these basic components, For example in our components directory there is `header`, `welcome` , `footer` folder where we wrote our different styled component. For example `welcome` component-

### Component folder structure
```text
|-- components
    ....
    ..
    |-- welcome ( welcome component folder )
        - welcome-one ( main demo welcome section )
        - welcome-two ( demo two welcome section )
        ...... ( and other )
    ...    
```

### Contact Page component
`inner-pages/contact-page/contact-page.component.html`

```text
|-- components
    ....
    ..
    |-- inner-pages ( all inner-pages folder )
        ......
        - contact-page ( contact-page component )
        ...... ( and other )
    ...    
```

```html
<div class="contact-page">
    <div class="main">
        <app-scrollup></app-scrollup>
        <app-header-one></app-header-one>
        <app-breadcrumb-contact></app-breadcrumb-contact>
        <section id="contact" class="contact-area bg-gray ptb_100">
            <div class="container">
                <div class="row">
                    <div class="col-12 col-md-10 col-lg-8">
                        <!-- Section Heading -->
                        <div class="section-heading">
                            <span class="d-inline-block rounded-pill shadow-sm fw-5 px-4 py-2 mb-3">
                                <i class="far fa-lightbulb text-primary mr-1"></i>
                                <span class="text-primary">Stay</span>
                                Tuned
                            </span>
                            <h2>Don't hesitate to contact us</h2>
                            <p class="d-none d-sm-block mt-4">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Laborum obcaecati dignissimos quae quo ad iste ipsum officiis deleniti asperiores sit.</p>
                            <p class="d-block d-sm-none mt-4">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Laborum obcaecati.</p>
                        </div>
                    </div>
                </div>
                <div class="row justify-content-between">
                    <div class="col-12 col-md-5">
                        <!-- Contact Us -->
                        <div class="contact-us">
                            <p class="mb-3">Contrary to popular belief, Lorem Ipsum is not simply random text. It has roots in a piece of classical Latin literature from 45 BC, making it over 2000 years old.</p>
                            <ul>
                                <li class="py-2">
                                    <a class="media" href="#">
                                        <div class="social-icon mr-3">
                                            <i class="fas fa-home"></i>
                                        </div>
                                        <span class="media-body align-self-center">Vestibulum nulla libero, convallis, tincidunt suscipit diam, DC 2002</span>
                                    </a>
                                </li>
                                <li class="py-2">
                                    <a class="media" href="#">
                                        <div class="social-icon mr-3">
                                            <i class="fas fa-phone-alt"></i>
                                        </div>
                                        <span class="media-body align-self-center">+1 230 456 789-012 345 6789</span>
                                    </a>
                                </li>
                                <li class="py-2">
                                    <a class="media" href="#">
                                        <div class="social-icon mr-3">
                                            <i class="fas fa-envelope"></i>
                                        </div>
                                        <span class="media-body align-self-center">exampledomain@domain.com</span>
                                    </a>
                                </li>
                            </ul>
                        </div>
                    </div>
                    <div class="col-12 col-md-6 pt-4 pt-md-0">
                        <!-- Contact Box -->
                        <div class="contact-box text-center">
                            <!-- Contact Form -->
                            <form id="contact-form" method="POST" action="assets/php/mail.php">
                                <div class="row">
                                    <div class="col-12">
                                        <div class="form-group">
                                            <input type="text" class="form-control" name="name" placeholder="Name" required="required">
                                        </div>
                                        <div class="form-group">
                                            <input type="email" class="form-control" name="email" placeholder="Email" required="required">
                                        </div>
                                        <div class="form-group">
                                            <input type="text" class="form-control" name="subject" placeholder="Subject" required="required">
                                        </div>
                                    </div>
                                    <div class="col-12">
                                        <div class="form-group">
                                            <textarea class="form-control" name="message" placeholder="Message" required="required"></textarea>
                                        </div>
                                    </div>
                                    <div class="col-12">
                                        <button type="submit" class="btn btn-lg btn-block mt-3"><span class="text-white pr-3"><i class="fas fa-paper-plane"></i></span>Send Message</button>
                                    </div>
                                </div>
                            </form>
                            <p class="form-message"></p>
                        </div>
                    </div>
                </div>
            </div>
        </section>
        <section class="section map-area">
            <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2485.596666220624!2d-0.16124461362595294!3d51.46556134684942!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x487605a25375dfb7%3A0xe0d9fa09dcf932a8!2s15%20Theatre%20St%2C%20Battersea%2C%20London%20SW11%205ND%2C%20UK!5e0!3m2!1sen!2sbd!4v1567427969685!5m2!1sen!2sbd" width="100" height="100" style="border:0;" allowfullscreen=""></iframe>
        </section>
        <app-footer-one></app-footer-one>
    </div>
</div>
```


## theme installtion
To install the theme you have to install [angular](https://cli.angular.io/) than go to the theme root dir where `package.json` located and use
```bash
npm install -g @angular/cli
```
it will install the packages.

After install process now you can run local server- local server port is 'http://localhost:4200' For developement start use
```bash
ng serve -o
```
## Build your theme
```bash
ng build --prod
```

## For deployment -- static server
First install
```bash
ng build --watch
ng build --aot
```
If you want to know more about static deployment please visit [Angular app deployment](https://angular.io/guide/deployment)

Enjoy your theme :)
