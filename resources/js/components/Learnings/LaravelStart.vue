<template>
    <div>
        <div class="card card-intro">

            <div class="card-body white-text text-center">

                <!--Grid row-->
                <div class="row d-flex justify-content-center">
                <img :src="artisan" style="width: 7rem; height: 7rem; border-radius: 100%"/>
                <!--Grid column-->
                <div class="col-md-6">
                    <p class="h5 mb-2">
                    This is Good Morning Blog
                    </p>
                    <p class="mb-0">The latest news from the world of internet technologies.</p>
                    <p>Author: Eliya Joseph</p>
                </div>
                <!--Grid column-->
                </div>
                <!--Grid row-->
            </div>
        </div>
            <!-- Intro -->
        <div class="container z-depth-1">
            <section class="p-md-3 mx-md-5">
                <div class="row d-flex justify-content-between align-items-center">
                <div class="col-md-6 mb-4">
                    <h2 class="font-weight-bold mb-3">Creating Laravel Application</h2>
                    <p class="text-muted pt-3">
                    Before diving in, we need first to know what is <strong class="text-warning">Laravel</strong>.<br />
                    Just in breaf, Laravel is a PHP web application framework with expressive, elegant syntax. Laravel has already laid the foundation — 
                    freeing you to create without sweating the small things.<br />
                    For full undersranding and installation, you can refer to <a target="_blank" href="https://laravel.com/docs/7.x" class="text-danger">Laravel official documentation</a>.
                    </p>
                </div>
                <div class="col-md-6 col-lg-4 d-flex justify-content-center mb-md-0 mb-5">
                    <img src="https://www.bootstrapdash.com/wp-content/uploads/2020/03/what-is-laravel.jpg" class="img-fluid" />
                </div>
                </div>
            </section>
            <section class="p-md-3 mx-md-5">
                <h2 class="font-weight-bold mb-3">Laravel App</h2>
                <p>Before creating a Laravel application, your first required to download and install <strong class="text-warning">composer</strong>
                    and add it to <strong class="badge badge-default shadow text-primary">PATH</strong>.<br />
                    You can download <a href="https://getcomposer.org/" class="text-primary" target="_blank">composer from here</a>
                </p>
                <div class="row d-flex justify-content-between align-items-center">
                    <div class="col-md-6">
                        <p>placing Composer's system-wide vendor bin directory in your <strong class="badge badge-default shadow text-primary">PATH</strong>
                            so the laravel executable can be located by your system. This directory exists
                            in different locations based on your operating system; however, some common locations are:
                        </p>
                        <p>You could also find the composer's global installation path by
                            running <em class="text-info shadow">composer global about</em>  and looking up from the first line.
                        </p>
                    </div>
                    <div class="col-md-6 col-lg-5 d-flex justify-content-center mb-md-0 mb-5">
                        <ul class="bg-light shadow p-3">
                            <li><strong class="text-danger">macOS:</strong> $HOME/.composer/vendor/bin</li>
                            <li><strong class="text-danger">Windows:</strong> %USERPROFILE%\AppData\Roaming\Composer\vendor\bin</li>
                            <li><strong class="text-danger">GNU / Linux Distributions: </strong>$HOME/.config/composer/vendor/bin or<br />
                                                        $HOME/.composer/vendor/bin
                            </li>
                        </ul>
                    </div>
                </div>

                <div class="row d-flex justify-content-between align-items-center pt-5">
                    <div class="col-md-6">
                        
                        <p>This tutorial only explain how to create laravel app using composer, for other ways you can  refer to <a href="https://laravel.com/docs/7.x" class="text-danger">Laravel official documentation</a>.<br />
                            You can install Laravel by issuing the Composer <em class="badge text-danger shadow">create-project</em> command in your terminal:
                        </p>
                        <p>will create a directory named <strong class="text-info shadow">blog</strong> containing a fresh Laravel installation with all of Laravel's dependencies already installed</p>
                    </div>
                    <div class="col-md-6 col-lg-5 d-flex justify-content-center mb-md-0 mb-5">
                        <img :src="create_project" class="img-fluid" />
                    </div>
                </div>
            </section>
            <section class="p-md-3 mx-md-5">
                <h2 class="font-weight-bold mb-3">Local Development Server</h2>
                <p>Once the project is created, change directory to where the project has been created. i.e, if 
                    the project was created in <em class="badge badge-danger shadow">htdocs</em> directory, 
                    and you type <em class="text-danger shadow">cd blog</em>, it should look like:
                </p>
                <img :src="project_directory" class="img-fluid" />
                <div class="p-3">
                    <p class="lead">If you have PHP installed locally and you would like to use PHP's built-in development
                        server to <strong class="badge text-danger shadow">serve</strong> your application, you may use the serve Artisan command. 
                        This command will start a development server at <strong class="badge shadow"><em class="text-danger"> http</em>://localhost:8000:</strong>
                    </p>
                    <p class="bg-light shadow p-3">
                        php artisan serve
                    </p>
                    <p>After typing the above command, visit your browser at 
                        <strong class="badge shadow"><em class="text-danger"> http</em>://localhost:8000</strong>
                        and you will see the page like this:
                    </p>
                    <img :src="artisan" class="img-fluid" />
                </div>
            </section>
        </div>
    </div>
    
</template>

<script>
export default {
    name: 'LaravelStart',
    data() {
        return {
            paths: '/dist/img/startLaravel/paths.png',
            create_project: '/dist/img/startLaravel/create-project.png',
            project_directory: '/dist/img/startLaravel/directory.png',
            artisan: '/dist/img/startLaravel/laravel-artisan.jpg',
        }
    }
}
</script>

<style scoped>
    img {
        box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
    }
    ul li {
        list-style-type: none;
    }
    .card {
         background-image: linear-gradient(to right, #2D48B1, #1C2331);
         color: #fff;
         padding: 3rem;
    }
</style>