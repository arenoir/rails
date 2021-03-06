*   Partial template name does no more have to be a valid Ruby identifier.

    There used to be a naming rule that the partial name should start with
    underscore, and should be followed by any combination of letters, numbers
    and underscores.
    But now we can give our partials any name starting with underscore, such as
    _🍔.html.erb.

    *Akira Matsuda*

*   Change the default template handler from `ERB` to `Raw`.

    Files without a template handler in their extension will be rendered using the raw
    handler instead of ERB.

    *Rafael Mendonça França*

*   Remove deprecated `AbstractController::Base::parent_prefixes`.

    *Rafael Mendonça França*

*   Default translations that have a lower precedence than a html safe default,
    but are not themselves safe, should not be marked as html_safe.

    *Justin Coyne*

*   Make possible to use blocks with short version of `render "partial"` helper.

    *Nikolay Shebanov*

*   Add a `hidden_field` on the `file_field` to avoid raise a error when the only
    input on the form is the `file_field`.

    *Mauro George*

*   Add an explicit error message, in `ActionView::PartialRenderer` for partial
    `rendering`, when the value of option `as` has invalid characters.

    *Angelo Capilleri*

*   Allow entries without a link tag in AtomFeedHelper.

    *Daniel Gomez de Souza*

Please check [4-2-stable](https://github.com/rails/rails/blob/4-2-stable/actionview/CHANGELOG.md) for previous changes.
