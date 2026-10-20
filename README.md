# Yang CHEN's academic website

Personal website: https://yangchen-econ.github.io

The website uses Jekyll and the AcademicPages theme. GitHub Pages builds and publishes the root of the master branch automatically after each push.

## Where to edit content

| Content | Source |
| --- | --- |
| About me | _pages/about.md |
| Research papers | _research/ |
| Conferences, visits, and summer schools | _conferences/ |
| Teaching | _teaching/ |
| CV download | files/YangCHEN_CV.pdf |
| Navigation links | _data/navigation.yml |
| Name, photo, affiliation, and contact details | _config.yml |
| Site styling | assets/css/main.scss and _sass/ |

## Adding an activity

Add a Markdown file in _conferences/ with YAML metadata between two lines containing three dashes. Set type to conference, visit, or summerschool. Supply title, date_start, date_end, venue, location, and event_url as appropriate. The activities page groups these records by type and sorts each group by its start date, newest first.

Summer schools belong in _conferences/ alongside the other activities. Each activity should have one source file.

## Adding a paper

Add a Markdown file in _research/. Supply title, paper_url, type, and a coauthors list with each coauthor's name and optional url. Use one pair of quotation marks around a name or title; an extra pair can prevent Jekyll from reading the entry.

## Previewing and publishing

With Ruby and Bundler installed, run:

```sh
bundle install
bundle exec jekyll serve
```

Open http://localhost:4000 to preview. After pushing a change, check the Pages build in the repository's Actions tab and then verify the live page.

The old courses and publications URLs redirect to the current activities and research pages. The CV aliases redirect to the real PDF. The jekyll-sitemap plugin generates sitemap.xml.

## Theme and license

Based on [AcademicPages](https://github.com/academicpages/academicpages.github.io), a fork of [Minimal Mistakes](https://github.com/mmistakes/minimal-mistakes). The original license is retained in LICENSE.
